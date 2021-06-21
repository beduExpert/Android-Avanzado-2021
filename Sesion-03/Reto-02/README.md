# Reto 02: Nuevo módulo

## Objetivo

* Implementar un módulo faltante mediante la reutilización del código generado por Hilt.
* Demostrar la imagen default en la lista de elementos.

## Desarrollo

Llegó el momento de agregar el módulo de **Planetas** a la app. 
Los requerimientos de este reto son los siguientes:

1. Para hacerlo crea un nuevo **Activity** llamado **PlanetsActivity**. Este debe realizar la llamada al servicio de **Planets** y debe mostrar los resultados. Asimismo, mantén la estructura y utiliza la inyección de dependencias. 
2. Agrega el nuevo módulo **Planets**. El usuario debe tener a su disposición la opción de elegir **People** o **Planets**. Al hacer clic sobre alguna de ellas deben realizarse las llamadas e importaciones necesarias para consultar el API y mostrar la lista de resultados. Además, la lista debe tener habilitado el **swipeRefresh**.
3. Una vez que hayas implementado el servicio, crea una dependencia que contenga una imagen de Star Wars; puedes agregar el **base64** o la URL. Inyecta esta imagen y después debes asignarla a la lista para que todos los elementos muestren esa imagen.

</br>

Las propuestas de solución son:

<img src="assets/01.png" width="50%"/>

<img src="assets/02.png" width="50%"/>

</br>
</br>

<details>
    <summary>Solución 1 - 2</summary>
    
Agregar **ResponsePlanetModel** con los datos del **Json**.
Nueva función a **ApiHelper**.

```Kotlin
suspend fun getPlanets(): Response<ResponsePlanetModel>
```

**ApiService**

```Kotlin
@GET("planets")
suspend fun getPlanets(): Response<ResponsePlanetModel>
```

Override a **ApiHelperImpl**

```Kotlin
override suspend fun getPlanets(): Response<ResponsePlanetModel> = apiService.getPlanets()
```

MainRepository

```Kotlin
suspend fun getPlanets() =  apiHelper.getPlanets()
```

Copiar paquete **main.people** a **main.planets** y modificar las referencias de **People** por **Planets**.

</details>

</br>

<details>
    <summary>Solución 3</summary>

**ApplicationModule**

```Kotlin
@Singleton
@Provides
@Named("provideImage")
fun provideImage() = "data:image/png;base64,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"
```

Modificar en **PeopleAdapter** y en **PlanetsAdapter** para que reciban el **imagePath** en el constructor y lo envíen como parámetro a cada elemento.

```Kotlin
class PlanetsAdapter(
    private val planet: ArrayList<Planet>,
    private val imagePath: String
) : RecyclerView.Adapter<PlanetsAdapter.DataViewHolder>() {

…

fun bind(model: Planet, imagePath: String) {
            itemView.textViewUserName.text = model.name
            itemView.textViewUserEmail.text = model.population
            Glide.with(itemView.imageViewAvatar.context)
                .load(imagePath)
                .into(itemView.imageViewAvatar)
}

…

holder.bind(planet[position], imagePath)
```

Inyectar dependencia en **PlanetsActivity** y en **PeopleActivity**.

```Kotlin
@Inject
@Named("provideImage")
lateinit var provideImage: String
```

Enviar dependencia inyectada al inicializar el constructor.

```Kotlin
adapter = PeopleAdapter(arrayListOf(), provideImage)
adapter = PlanetsAdapter(arrayListOf(), provideImage)
```

</details>

</br>

[Siguiente ](../Postwork/README.md)(Postwork)