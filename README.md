# Verificador de recibos de energía y servicios · v1.2

App web para **leer, verificar y comparar recibos** de agua, alcantarillado, energía, aseo y alumbrado. Lee PDF (sin internet) y fotos (con internet), compara mes a mes, revisa que las cuentas cuadren y exporta a Excel.

Todo se guarda **solo en tu dispositivo** (localStorage); no se envía nada a ningún servidor.

## Instalar en el celular

- **Android (Chrome):** abre la página y toca **Instalar app** (o menú ⋮ → *Instalar aplicación*).
- **iPhone / iPad (Safari):** toca **Compartir** → **Añadir a pantalla de inicio**.
- **Computador (Chrome / Edge):** ícono de instalar en la barra de direcciones.

## Publicar en GitHub Pages

1. Sube todos los archivos de esta carpeta a la raíz del repositorio.
2. En GitHub: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`**.
3. Abre `https://TU-USUARIO.github.io/NOMBRE-DEL-REPOSITORIO/` (debe ser HTTPS para poder instalarla).

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app completa (incluye el lector de PDF) |
| `manifest.webmanifest` | Nombre, colores e íconos de la app instalada |
| `sw.js` | Permite abrir la app sin internet |
| `icons/` | Íconos 192/512 px, versión *maskable*, iPhone y favicon |
| `favicon.ico` | Ícono de la pestaña del navegador |
| `.nojekyll` | Evita que GitHub Pages procese los archivos |

## Actualizar

Al modificar `index.html`, cambia `VERSION` en `sw.js` (por ejemplo `v1.2.2`) para que los dispositivos descarguen la nueva versión.

## Privacidad

El botón **Cargar mis 2 recibos de ejemplo** trae datos reales de dos recibos (valores y lecturas, sin nombre ni dirección). Si el repositorio es público, esos valores serán visibles.
