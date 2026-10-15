# Musimark

Libreto de ensayo para teatro musical: la letra va a tiempo con la canción, tus partes aparecen resaltadas según la categoría (voz o personaje) y podés saltar o repetir solo lo que te toca.

Es una app web instalable (PWA) de un solo archivo, sin dependencias ni build. Las letras, los tiempos y los audios se guardan en el navegador de cada dispositivo.

## Publicar con GitHub Pages

1. Settings → Pages.
2. Source: **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. Guardar. La app queda en `https://<usuario>.github.io/Musimark/`.
4. Abrir esa dirección en Chrome del teléfono → menú → **Instalar app**.

Para que Pages funcione con el repositorio privado hace falta un plan pago de GitHub. Con una cuenta gratis, hay que hacerlo público.

## Archivos

- `index.html`: la app completa.
- `manifest.webmanifest`, `icon-*.png`: datos para instalarla.
- `sw.js`: permite usarla sin conexión. Al publicar cambios, subir la versión de `V` en este archivo para que los teléfonos tomen lo nuevo.

## Pasar datos desde otra instalación

1. En la versión anterior: Copia de seguridad → Descargar archivo.
2. En Musimark: Copia de seguridad → Importar.
3. En cada canción: Ajustes → Agregar audios y elegir todos los mp3. Los que tienen el mismo nombre se reconectan solos.
