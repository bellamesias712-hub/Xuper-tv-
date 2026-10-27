# Xuper TV para Android TV / Google TV

Este es el proyecto Android Studio del prototipo Xuper TV. Empaqueta la interfaz HTML local dentro de una app Android con entrada en el launcher de Android TV/Google TV y navegación mediante control remoto.

## Crear el APK
1. Instala Android Studio en un computador y abre esta carpeta (`XuperTV-Android`).
2. Acepta la instalación del Android SDK si Android Studio lo solicita.
3. Espera a que termine la sincronización de Gradle.
4. Selecciona **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. El APK de prueba normalmente quedará en `app/build/outputs/apk/debug/app-debug.apk`.

## Instalar sin USB
1. Sube `app-debug.apk` a un almacenamiento/servidor HTTPS propio al que puedas acceder desde la TV.
2. En Android TV/Google TV instala una aplicación de descarga de archivos desde Google Play, o abre el enlace con un navegador compatible.
3. Descarga el APK y autoriza la instalación para esa aplicación si Android lo solicita en Ajustes > Apps > Acceso especial > Instalar apps desconocidas.
4. Abre Xuper TV desde tus aplicaciones.

También puedes instalarlo por red local usando ADB desde un computador en la misma Wi-Fi, activando primero Opciones de desarrollador y Depuración por red en la TV.

## Limitaciones del prototipo
- El catálogo, títulos y canales son de muestra.
- El reproductor muestra una ventana demostrativa; todavía no incluye proveedor de vídeo, playlist ni señales en vivo.
- No se incluye un APK precompilado en este ZIP porque compilarlo requiere Android SDK/Gradle. El código fuente sí está preparado para abrirse y compilarse en Android Studio.
- Para publicación en Google Play, revisar requisitos de Android TV, recursos gráficos de launcher y políticas vigentes.
