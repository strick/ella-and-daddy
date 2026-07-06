# EllaAndDaddy.com

Website for the **Ella and Daddy** children's picture books — currently featuring
*Can We Play Monster Now?* by Brian Strickland, illustrated by Okko W.

## Stack

Plain static HTML + CSS. No build step, no JavaScript, no frameworks.

- `index.html` — the whole site (single page)
- `css/styles.css` — storybook theme; palette pulled from the book cover art
- `images/` — cover (`monster-web.jpg`, resized for web; `monster.jpg` is the full-res original), sample spreads in `images/pages/`
- `favicons/` — favicon set + web manifest

Fonts: [Fredoka](https://fonts.google.com/specimen/Fredoka) (headings) and
[Nunito](https://fonts.google.com/specimen/Nunito) (body) via Google Fonts.

## Local preview

Any static file server works, e.g.:

```sh
python3 -m http.server 4173
```

## Deploy

Pushes to `main` deploy to Azure Static Web Apps via the pipeline in
`azure-static-web-apps-orange-island-0f210b90f.yml` (publishes the repo root as-is).
