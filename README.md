# Deutsch mit Josh

Sitio estático con el calendario semanal, las clases (diapositiva + plan de clase) y el plan de evaluación de 4 semanas.

## Estructura

- `index.html`: página principal
- `css/styles.css`: estilos
- `js/lessons.js`: datos de las clases (arreglo `LESSONS`) y generación de las cards
- `.nojekyll`: evita que GitHub Pages procese el sitio con Jekyll

## Publicar con GitHub Pages

1. Crea un repositorio en GitHub (por ejemplo `deutsch-con-josh`).
2. Sube todos los archivos de esta carpeta a la raíz del repositorio (incluido `.nojekyll`).
3. Ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guarda.
5. Espera 1–2 minutos. El sitio quedará en `https://TU-USUARIO.github.io/deutsch-con-josh/`.

## Antes de publicar

- Cambia `tucorreo@ejemplo.com` en `index.html` (sección de contacto).
- Pon los enlaces reales en la tabla «Evaluaciones abiertas» (`href="#"`).
- Las presentaciones de Google Slides deben estar compartidas con «Cualquier persona con el enlace» para que se vean incrustadas.

## Editar una clase

En `js/lessons.js`, cada clase tiene: `w` (semana y día), `t` (título), `m` (nivel y duración), `id` (ID de la presentación de Google Slides), `s` (diapositiva inicial) y `p` (los 7 apartados del plan). Para añadir una clase, copia un bloque y cambia esos valores.
