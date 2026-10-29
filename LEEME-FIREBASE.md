# Activar las cuentas de El Trienio (Firebase)

Mientras `firebase-config.js` diga `window.TRIENIO_FIREBASE = null;`, el juego funciona sin cuentas.

1. Entra a https://console.firebase.google.com y crea el proyecto "el-trienio" (Analytics opcional).
2. **Authentication › Comenzar › Método de acceso**: activa *Correo electrónico/contraseña* y *Google*.
3. **Authentication › Configuración › Dominios autorizados**: agrega el dominio donde publicas el juego (por ejemplo `tuusuario.github.io`).
4. **Firestore Database › Crear base de datos** en modo producción, ubicación `nam5` o `us-central`.
5. **Firestore › Reglas**: pega el contenido de `firestore.rules` y publica.
6. **Firestore › Índices**: no hace falta crear ninguno (el legado ordena por un solo campo).
7. **Configuración del proyecto › Tus apps › Web (</>)**: registra la app "El Trienio" y copia el objeto `firebaseConfig`.
8. Abre `firebase-config.js`, cambia `null` por ese objeto y sube los archivos.

La clave `apiKey` de Firebase no es secreta: identifica al proyecto. La seguridad la dan las reglas de `firestore.rules`.
