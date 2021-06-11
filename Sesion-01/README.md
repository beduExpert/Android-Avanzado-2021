
# :wave: Sesión 01: Firebase Authentication - Simplifica el inicio de sesión y el registro

## 🎯  Objetivo de la sesión:
Implementar Firebase Authentication en el código de la app para operar el registro e inicio de sesión con los métodos de Firebase.

## 🎯 Que aprenderán

- Implementación de firebase-auth en un proyecto.
- Gestión de usuarios sin código en el servidor.
- Simulación de registro y login con diferentes métodos de autenticación de Auth.

## ⚙ Requisitos

+ Haber revisado el prework de esta sesión
+ Cuenta de Google
+ Proyecto de Firebase
+ Android studio

## 🎩 Desarrollo

En esta sesión aprenderemos cuáles son los servicios de Firebase, las funciones que suma Authentication, y cómo se implementa dentro de un proyecto de Android para un registro e inicio de sesión enlazados con Auth, como la llamaremos también. 
Asimismo, se operará la app para verificar la funcionalidad del registro y del login mediante SMS,, correo y cuenta de Google.

Firebase Authentication proporciona servicios de backend, SDK y bibliotecas de IU preelaboradas que sirven para autenticar a los usuarios en tu app. Así, es posible la autenticación mediante contraseñas, números de teléfono, proveedores de identidad federada populares, como Google, Facebook y Twitter, y mucho más.


## ⚙ Configuración

### Firebase - Setup inicial

Antes de implementar firebase en nuestra app, debemos configurar un proyecto en la Firebase console. Para esto seguiremos los siguientes pasos:

- Abriremos [Firebase Console](https://console.firebase.google.com/?hl=es) con una cuenta google que poseamos y crearemos un proyecto nuevo.

    <img src="images/01.png" width="50%"/>

- Asignamos un nombre (en este caso, le llamaremos Bedu)

     Aceptaremos Google Analytics 

    <img src="images/02.png" width="50%"/>

- Seleccionamos México como *Ubicación de Analytics*, aceptaremos todos los términos y click en *Crear proyecto*

    <img src="images/03.png" width="50%"/>

- Listo, ya creamos nuestro Firebase Project

    <img src="images/04.png" width="50%"/>

</br>

## 📂 Organización de la clase

- [Ejemplo 01:  Implementar Firebase Authentication](./Ejemplo-01/README.md)
- [Ejemplo 02: Registrarse con correo y contraseña](./Ejemplo-02/README.md)
    - [Reto 01: Iniciar sesión](./Reto-01/README.md)
- [Ejemplo 03: Accede con número telefónico](./Ejemplo-03/README.md)
    - [Reto  02: Verificar y reenviar código](./Reto-02/README.md)
- [Postwork: Accede con Google](./Postwork/README.md)




