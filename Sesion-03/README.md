
# :wave: Sesi贸n 03: Dependencias - Simplifica el c贸digo

## 馃幆  Objetivo de la sesi贸n:

- Formular el c贸digo de la app con dependencias manuales o desde Dagger Hilt para construir una app con una arquitectura s贸lida.

## 馃幆 Qu茅 aprender谩n

- Creaci贸n de un proyecto Android con y sin la inyecci贸n de dependencias.
- Implementaci贸n de diversas herramientas para inyecci贸n de dependencias.
- Implementaci贸n de Dagger Hilt en proyecto de app Android.

## 鈿? Requisitos

+ Revisi贸n previa del Prework de la sesi贸n.
+ Android Studio.

## 馃帺 Desarrollo

En esta sesi贸n aprenderemos la inyecci贸n de dependencias, o DI, t茅cnica frecuente en programaci贸n y adecuada para el desarrollo de Android que es la base de una arquitectura s贸lida de apps.

Al programar una app las clases suelen requerir referencias a otras clases. Por ejemplo, una clase Car podr铆a necesitar una referencia a una clase Engine. A estas clases se les denomina dependencias. En el mismo ejemplo, la clase Car necesita una instancia de la clase Engine, de la que depende para ejecutarse.

En ese sentido, una clase puede obtener un objeto que necesita mediante alguna de las siguientes tres maneras:
1. La clase construye la dependencia que necesita. En el ejemplo anterior, Car crea e inicializa su propia instancia de Engine.
2. La clase la toma de otro lugar. Algunas API de Android, como los m茅todos get de Context y getSystemService(), funcionan de esta forma.
3. La clase la recibe como par谩metro. La app puede proporcionar estas dependencias cuando se construye la clase, o pasarlas a las funciones que necesitan cada dependencia. En el ejemplo anterior, el constructor Car recibe Engine como par谩metro.

En general, implementar la inyecci贸n de dependencias suma las siguientes ventajas:
- Reutilizaci贸n de c贸digo.
- Facilidad de refactorizaci贸n.
- Facilidad de prueba.

</br>

## 馃搨 Organizaci贸n de la clase

- [Ejemplo 01: Dependencias manuales](./Ejemplo-01/README.md)
- [Ejemplo 02: Implementar Dagger Hilt](./Ejemplo-02/README.md)
    - [Reto 01: Agregar dependencias](./Reto-01/README.md)
- [Ejemplo 03: Consumir API](./Ejemplo-03/README.md)
    - [Reto  02: Nuevo m贸dulo](./Reto-02/README.md)
- [Postwork: Nueva API y definici贸n de proyecto](./Postwork/README.md)