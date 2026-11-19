# A9 Viewer

App para ver las cámaras espía A9 (las que usan YsxLite o FtyCamPro) sin la app original: sin publicidad y sin usar el micrófono.

## Descargas

En [Releases](../../releases/latest):

- **A9Viewer-1.8.apk**: Android 10 o más nuevo.
- **A9Viewer-PC-1.1.zip**: Windows 10/11. Descomprimir y abrir `A9 Viewer.exe`. Trae su propio Java, no hay que instalar nada.

## Qué hace

Android:

- Video en vivo por la red de casa o por internet (con el ID de la cámara).
- Audio, visión nocturna, nitidez, rotar, espejo y foto.
- Cargar la cámara escaneando el QR de "compartir" de YsxLite.
- Detección de movimiento aunque la app esté cerrada: graba videos MP4 o saca fotos, guardados en privado dentro de la app. También puede dejar que la cámara grabe sola en su tarjeta SD.

PC (Windows):

- Video en vivo, audio, visión nocturna, nitidez, rotar, espejo y foto.
- Cargar la cámara escribiendo el ID o abriendo una imagen del QR.
- Detección de movimiento: graba videos MP4 o saca fotos en `Videos\A9 Viewer`, o deja que la cámara grabe sola en su SD. Con la ventana cerrada sigue vigilando desde la bandeja de Windows.

## Permisos en Android

- Red: para hablar con la cámara. Para verla por internet usa los servidores del fabricante de la cámara, igual que la app original.
- Cámara del celu: solo dentro del lector de QR.
- Notificaciones: para el aviso de "Vigilando la cámara".
- No usa el micrófono y no tiene publicidad.

## Notas

- La cámara atiende una sola conexión a la vez: si el celu está vigilando, la PC no puede verla al mismo tiempo.
- Usuario y clave por defecto de la cámara: `admin` / `admin`.
- El APK no viene de Play Store: Android pide permitir "instalar apps desconocidas".
- La primera vez que abrís la app de PC, Windows puede preguntar por el firewall: tocá **Permitir**.

## Créditos

- Protocolo de la cámara basado en el trabajo de [cam-reverse](https://github.com/DavidVentura/cam-reverse).
- Lector de QR: [ZXing](https://github.com/zxing/zxing) (Apache 2.0).
- Videos de la app de PC: [JCodec](https://github.com/jcodec/jcodec) (BSD).
