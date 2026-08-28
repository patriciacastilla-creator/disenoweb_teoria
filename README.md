# Machete de HTML y CSS

Apunte de consulta para la materia **Diseño Web — Nivel Fundamentos**.
Reúne la sintaxis de las cuatro clases, ejemplos de código listos para copiar,
un diccionario de errores frecuentes y un glosario.

## Publicarlo en GitHub Pages

1. En GitHub, **New repository** → nombre `machete-html-css` → **Public** → *Create*.
2. **Add file → Upload files** → arrastrá `index.html` y `README.md` → *Commit changes*.
3. **Settings → Pages** → en *Source* elegí **Deploy from a branch** → rama `main`, carpeta `/ (root)` → *Save*.
4. Esperá uno o dos minutos y recargá esa misma pantalla: aparece la dirección.

La dirección queda así:

```
https://TU-USUARIO.github.io/machete-html-css/
```

## Cómo está hecho

Un único archivo `index.html` con todo el CSS y el JavaScript adentro. No necesita
instalar nada ni compilar nada: se abre haciendo doble clic.

Usa dos recursos externos, que se descargan solos al abrir la página:

| Recurso | Para qué | Si no carga |
|---|---|---|
| Google Fonts | Las tipografías Bricolage Grotesque, Source Serif 4 y JetBrains Mono | La página se ve igual, con las tipografías del sistema |
| highlight.js (cdnjs) | Colorea la sintaxis de los bloques de código | El código se sigue leyendo, en un solo color |

Los dos se cargan por internet. Si en el aula la red los bloquea, la página
funciona igual: solo cambia el aspecto.

## Editarlo

Todo el contenido está dentro de `index.html`. Para agregar un tema nuevo:

1. Sumá el enlace en el índice lateral, dentro del `<nav class="side">`.
2. Sumá la sección en el cuerpo, copiando la estructura de cualquier otra:

```html
<section id="mi-tema" class="tema">
  <h3 class="tema-h"><span class="ab">&lt;</span>Mi tema<span class="ab">&gt;</span></h3>
  <p>...</p>
</section>
```

El `id` de la sección tiene que coincidir con el `href` del enlace del índice.
