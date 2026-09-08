# nahuelgomez.pro

Portfolio de **Nahuel Gómez Suárez**, full stack developer en Mar del Plata.
Sitio estático, sin build: un solo `index.html` con su CSS y su JS embebidos.

**En vivo:** https://nahuelgomez.pro

## Estructura

```
portfolio/
  index.html      el sitio completo — markup, estilos y scripts
  vercel.json     redirects, y el Content-Type de los .md
  llms.txt        índice para agentes y modelos de lenguaje
  perfil.md       perfil completo en español
  profile.md      perfil completo en inglés
  sitemap.xml     las cinco URLs públicas
  robots.txt      permisos de rastreo, con el sitemap declarado
  img/og.png      imagen de preview al compartir el enlace (1200×630)
  img/ screenshots/  capturas de los proyectos
```

## Cómo está armado el sitio

- **Hero fijo** que se desvanece mientras sube el contenido de abajo.
- **Proyectos**: barra lateral pegajosa con el índice, y cada proyecto ocupa
  una pantalla. El ancho del pliego se calcula a partir del alto libre
  (`min(calc((100svh - 35rem) * 1.6), 62%)`) para que la tarjeta entre siempre
  sin deformar la proporción de las capturas. Los sistemas se embeben
  corriendo en vivo en iframes.
- **Cierre** (stack, sobre mí, hablemos): las tres secciones dejan de apilarse
  y se recorren como una escena fija de 435vh. Cada una entra, se sostiene y
  se va entera antes de la siguiente; en el hueco no queda nada en pantalla y
  una bandada dibujada en canvas se dispara, así el corte se siente como un
  salto y no como un scroll.
- **Visor del CV** en overlay, para leerlo sin descargarlo.
- Todo esto se desactiva por debajo de 900px de ancho o con
  `prefers-reduced-motion`: ahí el sitio se lee apilado, como cualquier otro.

## Para agentes y modelos de lenguaje

El sitio es scroll animado e iframes, así que un rastreador ve poco texto.
Por eso el contenido está también en Markdown, enlazado desde el `<head>` con
`rel="alternate"` y declarado en el JSON-LD:

- [`/llms.txt`](https://nahuelgomez.pro/llms.txt) — índice, según la convención de [llmstxt.org](https://llmstxt.org)
- [`/perfil.md`](https://nahuelgomez.pro/perfil.md) — perfil completo en español
- [`/profile.md`](https://nahuelgomez.pro/profile.md) — perfil completo en inglés

## Desarrollo

No hay build ni dependencias. Se edita `portfolio/index.html` y se sirve
cualquier archivo estático:

```bash
python -m http.server 8000 --directory portfolio
```

## Despliegue

Vercel, con Root Directory apuntando a `portfolio/`:

```bash
vercel --prod
```

`www.nahuelgomez.pro` y `portfolio-ngs.vercel.app` redirigen con 308 al
dominio pelado, que es el canónico.
