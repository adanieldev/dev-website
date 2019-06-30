---
layout: "post"
title: "Firebase: Login Google en Android"
categories: android firebase
permalink: /:categories/login-google
---
Implementarás un login con Google en Firebase en tu aplicación Android. Además obtendrás la información del usuario directamente desde Firebase, nombre, correo y fotografía.

### Aprenderás

* Implementar un Login Google en Firebase
* Obtener información del usuario directamente desde Firebase

### Requisitos
* Haber implementado Login con Google en Android

## 1. Configuración
`build.gradle` del módulo

Las versiones pueden cambiar rápidamente, se debe considerar usar la misma versión que play-services-auth

## 2. Implementación

`FirebaseAuth` & `ListenerFirebaseAuth.AuthStateListener` es el oyente que se encarga de avisarnos cuando estamos autenticados o no. 
Atributos en la *Activity* que se necesite manejar la autenticación.

Inicialización en el método `onCreate()`

Empezar a escuchar en el método `onStart()` de la *Activity*

Terminar de escuchar en el método `onStop()` de la *Activity*

## 3. Modificaciones

Adición del método `requestIdToken()` al GoogleSignInOptions

Método de autenticación con Firebase

Llamado luego de que la autenticación con Google fue exitosa.

## 4. Información del usuario

Se puede acceder al usuario actual desde cualquier parte de nuestra aplicación mediante el método getCurrentUser() del FirebaseAuth.
Si el método `getCurrentUser()` es null nadie se autenticó en la aplicación.

## 5. Cerrar sesión y revocar acceso

Basta con usar el método `signOut()` del `FirebaseAuth` en cualquier parte de nuestra aplicación seguida del cierre de sesión o revoco de acceso de Google.

## El código

Código completo en:

*  [Repositorio en GitHub](https://github.com/adanieldev/FirebaseGoogleSignInAndroid) 
*  [Descargar código](https://github.com/adanieldev/FirebaseGoogleSignInAndroid/archive/master.zip) 