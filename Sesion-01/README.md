
# :wave: Sesi贸n 01: Firebase Authentication - Simplifica el inicio de sesi贸n y el registro

## 馃幆  Objetivo de la sesi贸n:
Implementar Firebase Authentication en el c贸digo de la app para operar el registro e inicio de sesi贸n con los m茅todos de Firebase.

## 馃幆 Qu茅 aprender谩n

- Implementaci贸n de firebase-auth en un proyecto.
- Gesti贸n de usuarios sin c贸digo en el servidor.
- Simulaci贸n de registro y login con diferentes m茅todos de autenticaci贸n de Auth.

## 鈿? Requisitos

+ Revisi贸n previa del prework de esta sesi贸n
+ Cuenta de Google
+ Proyecto de Firebase
+ Android studio

## 馃帺 Desarrollo

En esta sesi贸n aprenderemos cu谩les son los servicios de Firebase, las funciones que suma Authentication, y c贸mo se implementa dentro de un proyecto de Android para un registro e inicio de sesi贸n enlazados con Auth, como la llamaremos tambi茅n. 
Asimismo, se operar谩 la app para verificar la funcionalidad del registro y del login mediante SMS,, correo y cuenta de Google.

Firebase Authentication proporciona servicios de backend, SDK y bibliotecas de IU preelaboradas que sirven para autenticar a los usuarios en tu app. As铆, es posible la autenticaci贸n mediante contrase帽as, n煤meros de tel茅fono, proveedores de identidad federada populares, como Google, Facebook y Twitter, y muchos m谩s.


## 鈿? Configuraci贸n

### Firebase - Setup inicial

Antes de implementar firebase en nuestra app, debemos configurar un proyecto en la Firebase console. Para ello deben realizarse los siguientes pasos:

1. Abrir Firebase Console mediante una cuenta google que poseamos.
2. Crear un proyecto nuevo.

    <img src="images/01.png" width="50%"/>

3. Asignar un nombre al proyecto. En este caso se le llamar谩 "Bedu".
4. Aceptar la habilitaci贸n de Google Analytics para el proyecto.

    <img src="images/02.png" width="50%"/>

5. Seleccionar M茅xico como ubicaci贸n Analytics, hacer clic en los recuadros para aceptar todos los t茅rminos, y finalmente hacer clic en Crear proyecto.

    <img src="images/03.png" width="50%"/>

Y listo, ya creamos nuestro Firebase Project.

<img src="images/04.png" width="50%"/>

</br>

## 馃搨 Organizaci贸n de la clase

- [Ejemplo 01:  Implementar Firebase Authentication](./Ejemplo-01/README.md)
- [Ejemplo 02: Registrarse con correo y contrase帽a](./Ejemplo-02/README.md)
    - [Reto 01: Iniciar sesi贸n](./Reto-01/README.md)
- [Ejemplo 03: Accede con n煤mero telef贸nico](./Ejemplo-03/README.md)
    - [Reto  02: Verificar y reenviar c贸digo](./Reto-02/README.md)
- [Postwork: Accede con Google](./Postwork/README.md)




