# 한국어 말 - GitHub Pages

Este paquete está preparado para subirlo a GitHub y publicar la web con GitHub Pages.

## Archivos incluidos
- `index.html`: app principal ya actualizada
- `manifest.webmanifest`: configuración PWA
- `sw.js`: service worker para caché básica
- `icons/`: iconos y favicon basados en la bandera de Corea
- `.nojekyll`: evita procesado innecesario en GitHub Pages

## Despliegue en GitHub Pages
1. Crea un repositorio nuevo en GitHub.
2. Sube todos los archivos de este paquete manteniendo la misma estructura.
3. En GitHub ve a **Settings > Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**.
5. Selecciona la rama **main** y la carpeta **/(root)**.
6. Guarda los cambios.
7. Tras unos minutos, la web quedará publicada.

La URL tendrá este formato:
`https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/`

## Instalación como app
- **iPhone/iPad (Safari):** Compartir → Añadir a pantalla de inicio
- **Android (Chrome):** menú → Instalar app / Añadir a pantalla principal
- **PC (Chrome/Edge):** icono de instalar en la barra de direcciones

## Nota
El botón **Actualizar web** sigue disponible dentro de la barra principal de controles de la app.
