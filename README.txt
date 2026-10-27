TESTPRO - proyecto Android para compilar APK mediante GitHub Actions

Este proyecto envuelve la versión web de TestPro en una aplicación Android WebView y empaqueta el HTML localmente en la app. No necesita conexión para abrir el cuestionario incluido, siempre que la propia página no dependa de recursos externos.

COMO OBTENER EL APK SIN INSTALAR ANDROID STUDIO
1. Crea una cuenta en https://github.com/ si no tienes una.
2. Crea un repositorio nuevo llamado TestPro (puede ser privado).
3. En el repositorio, usa Add file > Upload files y sube el CONTENIDO de esta carpeta (incluida la carpeta oculta .github).
4. Pulsa Commit changes.
5. Abre la pestaña Actions. Si pregunta, habilita GitHub Actions.
6. Selecciona “Build TestPro APK” y pulsa Run workflow.
7. Espera a que termine con una marca verde. Abre la ejecución y, al final, descarga el artefacto “TestPro-debug-APK”.
8. Descomprime el ZIP descargado; dentro estará app-debug.apk.
9. Pasa el APK al teléfono Android, ábrelo y permite instalar aplicaciones desde esa fuente si Android lo solicita.

NOTAS
- Este es un APK de depuración, adecuado para pruebas personales; no está firmado como versión de publicación de Google Play.
- No subas claves privadas ni contraseñas al repositorio.
- Para subir archivos por la web, asegúrate de incluir .github/workflows/build-apk.yml. Si el navegador no muestra la carpeta oculta, crea ese archivo desde Add file > Create new file con esa ruta.
