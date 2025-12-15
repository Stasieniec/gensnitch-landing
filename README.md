# GenSnitch Landing Site

Minimal landing page for the GenSnitch Chrome extension.

## Development

```bash
npm install
npm run dev
```

Open [http://localhost:4321](http://localhost:4321)

## Build

```bash
npm run build
npm run preview  # preview production build locally
```

Output: `dist/`

---

## Cloudflare Pages Deployment

### Setup

1. Connect your repo to Cloudflare Pages
2. Configure build settings:
   - **Framework preset:** Astro
   - **Root directory:** _(leave empty)_
   - **Build command:** `npm ci && npm run build`
   - **Output directory:** `dist`

### Chrome Web Store URLs

Once deployed, use these URLs in your Chrome Web Store listing:

| Field | URL |
|-------|-----|
| Website | `https://<project>.pages.dev/` |
| Privacy policy | `https://<project>.pages.dev/privacy` |

Replace `<project>` with your Cloudflare Pages project name.

### Custom Domain (Optional)

1. Go to your Pages project → Custom domains
2. Add your domain (e.g., `gensnitch.dev`)
3. Update DNS as instructed
4. Update `site` in `astro.config.mjs` to match
