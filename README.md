# Taller Web

Aplicación interactiva en español para aprender a crear una página web con **HTML**, **CSS** y **JavaScript**. Tiene un editor con vista previa en vivo y cuatro lecciones.

Todo está en un solo archivo: `index.html`. No necesita instalar nada.

## Cómo abrirla

1. Descarga `index.html`.
2. Haz doble clic en el archivo. Se abre en tu navegador.

Funciona sin conexión a internet. Solo las tipografías (Inter, Space Grotesk y JetBrains Mono) se cargan desde Google Fonts; sin conexión se usa la letra del sistema.

## Qué incluye

| Lección | Tema | Qué se practica |
|---|---|---|
| 1. HTML | La estructura | Títulos, párrafos, listas, enlaces e imágenes |
| 2. CSS | El aspecto | Colores, tipografía, espacios, esquinas redondeadas y flexbox |
| 3. JavaScript | La interacción | Variables, eventos, `getElementById` y `textContent` |
| 4. Proyecto | Todo junto | Una lista de tareas con tema claro y oscuro |

Cada lección tiene una explicación corta, los conceptos clave y unos retos para probar.

## Cómo se usa

- Elige una lección en la parte superior.
- Edita el código en las pestañas `index.html`, `estilos.css` y `script.js`.
- La vista previa se actualiza mientras escribes.
- La tecla **Tab** inserta dos espacios dentro del editor.
- **Restablecer esta lección** devuelve el código de ejemplo original.
- **Copiar archivo completo** une el HTML, el CSS y el JavaScript en un solo documento listo para guardar.

Los cambios que hagas en el editor no se guardan al cerrar la página. Copia tu código antes de salir.

## Cómo publicar tu propia página

1. Pulsa **Copiar archivo completo** en la lección que quieras.
2. Pégalo en un editor de texto (Bloc de notas, VS Code) y guárdalo como `index.html`.
3. Ábrelo con doble clic para verlo en tu navegador.
4. Para ponerlo en internet, sube el archivo a un servicio gratuito como GitHub Pages o Netlify.

## Cómo personalizarla

- **Colores:** están al inicio de la etiqueta `<style>`, en el bloque `:root`. Cada lección usa uno: `--html`, `--css`, `--js` y `--final`.
- **Modo oscuro:** los mismos colores se redefinen en los bloques de `prefers-color-scheme: dark` y `data-theme="dark"`.
- **Lecciones:** están en la lista `LESSONS` dentro del `<script>`. Cada una tiene `name`, `intro`, `concepts`, `challenge` y el código de ejemplo (`code.html`, `code.css`, `code.js`).
- **Añadir una lección:** agrega un objeto nuevo a `LESSONS` y un color con el mismo nombre que su `id` (por ejemplo `--mi-leccion`).

## Estructura del proyecto

```
index.html   La aplicación completa (HTML, CSS y JavaScript)
README.md    Este archivo
```

## Tecnologías

HTML, CSS y JavaScript sin librerías ni dependencias. La vista previa usa un `iframe` con `srcdoc` para ejecutar el código del editor de forma aislada.
