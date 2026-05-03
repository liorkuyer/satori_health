# TestDynamics — Astro Static Site

Faithful port of testdynamics.net to Astro, matching the original theme exactly:
- **Font**: Manrope (all weights)
- **Gradient**: `linear-gradient(270deg, #9281ff 0%, #fe3e70 52.55%, #ff6142 100%)`
- **Dark color**: `#2a3342`
- **Darker**: `#101225`
- **Light bg**: `#f7f8f9`

## Pages
| Route | File |
|---|---|
| `/` | `src/pages/index.astro` |
| `/platform` | `src/pages/platform.astro` |
| `/about` | `src/pages/about.astro` |
| `/news` | `src/pages/news.astro` |
| `/contact` | `src/pages/contact.astro` |
| `/request-demo` | `src/pages/request-demo.astro` |

## Run locally

```bash
npm install
npm run dev
# → http://localhost:4321
```

## Deploy to Cloudflare Pages

1. Push to GitHub
2. Connect repo in [pages.cloudflare.com](https://pages.cloudflare.com)
3. Build command: `npm run build`
4. Output directory: `dist`

## Deploy to Netlify

Forms use `data-netlify="true"` — they work automatically on Netlify.

1. Push to GitHub
2. Connect in Netlify dashboard
3. Build command: `npm run build`
4. Publish directory: `dist`

## TODO

- [ ] Download all images from `testdynamics.net/wp-content/uploads/` into `public/images/` and update src paths
- [ ] Add individual blog post pages under `/news/[slug].astro`
- [ ] Add algorithm/product detail pages
- [ ] Add terms and privacy pages
- [ ] Wire up contact forms (Netlify Forms or Formspree)
- [ ] Add Open Graph meta tags
