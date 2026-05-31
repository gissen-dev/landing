# gissen.dev — coming-soon page

A single-page placeholder for [Gissen](https://github.com/gissen-dev), the open-source
headless visual editor for Vue. Built with Vue 3 + TypeScript + Vite.

## Develop

```sh
npm install
npm run dev      # http://localhost:5173
npm run build    # type-check + production build → dist/
npm run preview  # serve the production build locally
```

## Deploy (Cloudflare Pages)

Connect the repo in the Cloudflare dashboard, or use Wrangler:

| Setting               | Value           |
| --------------------- | --------------- |
| Framework preset      | Vue / Vite      |
| Build command         | `npm run build` |
| Build output directory| `dist`          |

```sh
# one-off direct upload (no Git integration needed)
npm run build
npx wrangler pages deploy dist --project-name=gissen
```

Then point the `gissen.dev` custom domain at the Pages project in the dashboard.
`public/_headers` adds security + caching headers; `robots.txt` and `sitemap.xml`
are served from the site root for SEO.

## Contact

There's no signup form yet — the page links to the GitHub org and shows
`hello@gissen.dev` in the footer. Both the contact email and the GitHub URL are
constants at the top of `src/App.vue`.
