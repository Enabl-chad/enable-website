# enabl.co

Marketing site for Enabl Development, built with [Astro](https://astro.build).

## Project structure

```
/
├── public/            static assets served as-is (favicon, og-image, etc.)
├── src/
│   ├── components/    shared components — Nav, Footer, Button, Card, GradientText, WaveformMark
│   ├── layouts/        shared page layout(s)
│   └── pages/          one .astro file per route
└── astro.config.mjs
```

## Commands

Run these from the project root in a terminal with internet access:

| Command           | Action                                       |
| :----------------- | :-------------------------------------------- |
| `npm install`       | Install dependencies                          |
| `npm run dev`       | Start local dev server at `localhost:4321`    |
| `npm run build`     | Build production site to `./dist/`            |
| `npm run preview`   | Preview the build locally before deploying    |

## Deploy

Deployed via Cloudflare Pages, connected to this repo's `main` branch. Custom domain
attaches as `www.enabl.co` (CNAME) with a redirect from the bare `enabl.co` — see the
build plan for why (GoDaddy DNS, apex-domain limitation).
