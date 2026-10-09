# Sello QR

Generador de códigos QR (enlaces, teléfonos, redes sociales o texto libre) con color, forma, tamaño y logo personalizables. Un único archivo `index.html`, sin dependencias externas ni backend: todo se genera en el navegador de quien lo usa.

## Publicarlo en GitHub Pages

1. Crea un repositorio nuevo en GitHub (puede ser público o privado con GitHub Pro/Team).
2. Sube `index.html` a la raíz del repositorio (puedes arrastrarlo desde la web de GitHub con "Add file → Upload files", o por línea de comandos):
   ```bash
   git init
   git add index.html
   git commit -m "Sello QR"
   git branch -M main
   git remote add origin https://github.com/TU-USUARIO/TU-REPO.git
   git push -u origin main
   ```
3. En el repositorio, ve a **Settings → Pages**.
4. En "Build and deployment", elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guarda.
5. Espera uno o dos minutos: GitHub te dará la URL pública, algo como
   `https://TU-USUARIO.github.io/TU-REPO/`.

No necesitas build step, ni Node, ni ningún paquete: es HTML/CSS/JS plano.

## Notas

- Con logo, el nivel de corrección de errores sube automáticamente al máximo (H), y si el código es muy pequeño el logo se reduce un poco para que se siga leyendo.
- Antes de imprimir o compartir un código, escanéalo con el celular para confirmar que abre donde esperas.
- Todo el procesamiento (colores, forma, logo, descarga) ocurre en el navegador; nada se envía a un servidor.
