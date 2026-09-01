# EngPath

A self-contained, single-file engineering roadmap platform. No build step,
no dependencies — `index.html` contains everything: markup, styles, script
and the full roadmap dataset.

## Deploying

### Via GitHub → Netlify
1. Push this folder to a GitHub repository (as-is, `index.html` at the root).
2. In Netlify: **Add new site → Import an existing project → GitHub** → select the repo.
3. Build settings: leave the build command **empty** and set the publish
   directory to `/` (the repo root). There is nothing to build — this is a
   static file.
4. Deploy.

### Direct drag-and-drop (no GitHub)
Go to https://app.netlify.com/drop and drag this folder onto the page.

## Notes
- No `package.json`, no `npm install`, no build tooling — that's intentional.
  If Netlify tries to run a build command, clear it in **Site settings →
  Build & deploy → Build settings**.
- `index.html` is the required filename for Netlify to serve it at the
  site's root URL.
