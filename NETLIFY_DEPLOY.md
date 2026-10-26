# Netlify Deployment — Business Connect

## Recommended deployment

Use **Netlify → Add new project → Import an existing project** and connect the repository containing this project.

Build settings:
- Build command: `npm run build`
- Publish directory: `dist`
- Node version: `22`

The included `netlify.toml` already contains these settings and the SPA redirect.

## Important
Do **not** use Netlify's manual drag-and-drop with the project source ZIP if you expect Netlify to run the Vite build. Manual deployment expects already-built static files.

If using manual deployment, first run:

```bash
npm install
npm run build
```

Then drag the **dist** folder to Netlify Drop.

## SPA routing

`netlify.toml` redirects all application routes to `/index.html`, so routes such as `/dashboard`, `/directory`, `/b2b`, `/b2c`, and `/rfq-board` do not produce Netlify 404 pages after a successful deployment.
