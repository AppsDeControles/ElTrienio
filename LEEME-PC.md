# El Trienio en PC

## Instalar en Windows o Mac (gratis, ya funciona)
1. Abre el juego en Chrome o Edge: https://appsdecontroles.github.io/ElTrienio/
2. En la portada toca **INSTALAR**, o el ícono de instalar que aparece a la derecha de la barra de direcciones.
3. Queda como programa con su ícono, en su propia ventana, y se actualiza solo cuando subes cambios a GitHub.

## Publicar en Microsoft Store
1. Crea tu cuenta de desarrollador en https://partner.microsoft.com/dashboard (cuenta individual, pago único de unos 19 USD).
2. En el Partner Center: **Apps y juegos → Nuevo producto → Aplicación MSIX o PWA**, y reserva el nombre "El Trienio".
3. Entra a https://www.pwabuilder.com, pega la dirección del juego y toca **Start**.
4. Toca **Package For Stores → Windows**. Copia los datos que te pide (Package ID, Publisher ID y Publisher display name) de **Administración de productos → Identidad del producto** en el Partner Center.
5. Descarga el paquete (.zip). Adentro vienen archivos `.msixbundle`.
6. En el Partner Center crea un **Envío**: sube el `.msixbundle`, llena precio (gratis), clasificación de edad (cuestionario IARC), descripción, capturas de pantalla (mínimo 1 de 1366×768) y la política de privacidad.
7. Envía a certificación. Suele tardar de 1 a 3 días.

**Política de privacidad:** la tienda la pide porque el juego tiene cuentas (Firebase). Puede ser una página sencilla en GitHub Pages que diga qué datos se guardan (correo, nombre y partida) y para qué.
