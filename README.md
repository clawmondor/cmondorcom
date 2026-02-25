# cmondor.com

Personal brand and portfolio site for [Chris Mondor](https://cmondor.com) — Software, DevOps & Infrastructure Engineer.

## Stack

- Plain HTML5 + CSS (no frameworks, no build step)
- Hosted on [Netlify](https://netlify.com) with continuous deployment from `main`
- Google Analytics via gtag.js (G-3HNB8D27RV)

## Local Development

Requires [Netlify CLI](https://docs.netlify.com/cli/get-started/) installed globally.

```bash
npm run dev
```

Serves the site at `http://localhost:8888` with Netlify headers active.

## Deployment

Pushes to `main` automatically deploy to production via Netlify.

- **Production**: https://cmondorcom.netlify.app
- **Dashboard**: https://app.netlify.com/projects/cmondorcom
