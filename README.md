# Midnight

**ES** — Tema azul noche para Kino, en teléfono y Android TV, inspirado en Disney+: fondo oscuro con degradado, acento azul, tarjetas con borde blanco fino al enfocar, héroe enmarcado, riel flotante y un logo propio (aro con punto de acento). Proyecto independiente y no oficial, sin relación con Disney.

**EN** — A midnight-blue Kino theme for phone and Android TV, Disney+-inspired: dark gradient background, blue accent, cards with a thin white border on focus, a framed hero, a floating rail and its own logo (ring with an accent dot). Independent, unofficial project, not affiliated with Disney.

![Teléfono / Phone](docs/screenshots/phone-home.jpg)
![TV](docs/screenshots/tv-home.png)
![Menú TV / TV menu](docs/screenshots/tv-menu.png)

## Instalar / Install

En Kino: **Plugins ▸ Agregar**, escribe / type: `ElCompitaDanny/kino-plugin-theme-midnight`.
Luego activa el tema en **Ajustes ▸ App ▸ Apariencia** (o desde el aviso al instalar).

Requiere Kino 0.9.87 o posterior (`apiVersion` 26); recomendado 0.9.93.
Requires Kino 0.9.87 or later (`apiVersion` 26); 0.9.93 recommended.

## Personalizable / Adjustable

Acento (4 tonos de azul), redondeo de tarjetas, escala tipográfica y fondo.

> **Nota sobre el color de acento.** Kino descarta el tema si el acento no tiene contraste suficiente con el texto blanco (en pruebas, un azul `#2F8CFF`, de 3.3:1, hizo que Kino volviera al tema rojo por defecto). Si cambias el acento, usa azules con contraste de 4.5:1 o más sobre blanco.
> *Kino fell back to its default red theme when the accent had too little contrast with white text. Keep any accent at 4.5:1 or higher.*

## Archivos / Files

- `kino-plugin.json`: el tema, como datos (no ejecuta código) / the theme, as data.
- `plugin.js`: entrada mínima que no hace nada / minimal no-op entry.
- `icon.png`: icono del plugin / plugin icon.

No usa imágenes externas ni assets.

## Validación / Validation

Con Node 18+ y el [SDK oficial](https://github.com/kinotvapp/kino-plugin-sdk): `node sdk/validate.mjs .`
Probado a mano en teléfono y Android TV (Kino 0.9.93). El validador oficial aún no se ha ejecutado.

## Límite del tema / Scope

Un tema cambia los tokens y capas que Kino expone; no altera el catálogo ni el orden o contenido de las filas.

## Créditos / Credits

Estructura basada en el tema de ejemplo [Crimson](https://github.com/kinotvapp/kino-plugin-theme-crimson), de kinotvapp. El logo vectorial es propio.
