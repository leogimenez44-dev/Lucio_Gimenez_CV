# README for Lucio Gimenez CV Project

Este proyecto tiene como objetivo generar un currículum vitae (CV) en formatos DOCX y PDF a partir de un archivo HTML. Utiliza GitHub Actions para automatizar el proceso de generación cada vez que se realiza un push en la rama `main`.

## Estructura del Proyecto

- **.github/workflows/generate-cv.yml**: Workflow de GitHub Actions que se activa al hacer push en la rama `main`. Instala las dependencias necesarias (`pandoc`, `wkhtmltopdf`, `libreoffice`), genera un archivo DOCX y un PDF a partir de `index.html`, y realiza un commit y push de los archivos generados si hay cambios.

- **index.html**: Página principal del CV. Contiene la estructura HTML y el contenido que se convertirá en DOCX y PDF.

- **assets/css/styles.css**: Archivo que contiene los estilos CSS aplicados a `index.html`, definiendo la apariencia del CV.

## Uso

1. Asegúrate de tener los archivos necesarios en el repositorio.
2. Realiza un push en la rama `main` para activar el workflow de GitHub Actions.
3. Los archivos generados (`Lucio_Gimenez_CV.docx` y `Lucio_Gimenez_CV.pdf`) se agregarán automáticamente al repositorio si hay cambios.

## Requisitos

- GitHub Actions debe estar habilitado en el repositorio.
- Las dependencias se instalarán automáticamente durante el proceso de CI/CD.

## Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar el proyecto, por favor abre un issue o un pull request.