# FUNCAF Archivo Digital — interfaz

Este proyecto es una interfaz web estática (HTML, CSS y JavaScript) preparada para publicar en GitHub Pages.

## Qué funciona en esta versión
- Interfaz adaptable a móvil y PC.
- Selección de archivos y arrastrar/soltar.
- Lista de archivos seleccionados y tamaños, retirar archivos y limpiar selección.
- No se suben archivos a internet en esta versión.

## Importante: almacenamiento real para archivos grandes
GitHub Pages sirve la página, pero no almacena los archivos cargados. Para carga real de archivos grandes, se puede integrar Cloudflare R2 mediante un backend Cloudflare Worker que gestione autenticación y multipart uploads. Nunca expongas claves de API o credenciales en `app.js`.

## Publicar en GitHub Pages
1. Crea un repositorio en GitHub y sube `index.html`, `styles.css` y `app.js`.
2. En el repositorio, entra en **Settings → Pages**.
3. En Source, selecciona **Deploy from a branch**, elige `main` y `/ (root)`.
4. Guarda y espera el enlace de Pages.

## Próxima etapa
Conectar Cloudflare R2 y un Worker con URLs o multipart upload autorizados para habilitar almacenamiento real. Verifica las cuotas vigentes del proveedor antes de subir archivos.
