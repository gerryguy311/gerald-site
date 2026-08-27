# gerald.media

Personal speaker resources site for Gerald Auger, PhD. Static HTML, deployed on
Cloudflare Workers static assets, source of truth in this repo.

## Layout

```
public/          everything served at the domain
  index.html     the page
  assets/        headshots, action shots, slide PDFs
wrangler.jsonc   Cloudflare config
```

## Deploy

```
npx wrangler deploy
```

Once the GitHub repo is connected in Workers Builds, every push to `main`
deploys automatically and the command above is only needed for one-off pushes.

## Local preview

```
npx wrangler dev
```

## Before launch

- Remove the `<meta name="robots" content="noindex, nofollow">` line in
  `public/index.html`
- Fill in the `TODO` comments in `public/index.html`
- Drop real images into `public/assets/`
