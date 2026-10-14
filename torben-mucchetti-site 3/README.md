# Torben Mucchetti — Artist Site + Editing Dashboard

## What's included
- Site: `index.html`, `assets/`
- Editable content: `content/shows.json`, `releases.json`, `site.json`, `photos.json`
- Pages CMS dashboard config: `.pages.yml`

## Publish / enable your dashboard
1. Create a GitHub repository (for example `torben-mucchetti-site`) and upload **the contents of this folder** to the repository root, including the hidden `.pages.yml` file.
2. Connect the repository to Netlify: Add new project → Import from Git → GitHub → select repository. For this plain HTML site there is no build command; set publish directory to `.`.
3. Go to https://app.pagescms.org, sign in with GitHub, install/authorize Pages CMS for your repository, and choose your site repo. Your four editorial areas are **Shows & Flyers**, **Music Releases**, **Bio & Contact**, and **Photo Gallery**.
4. Make an edit in Pages CMS and save. Pages CMS commits the change to GitHub; Netlify auto-deploys on the repo update. The live site then loads the new content.
5. Optionally connect your custom domain in Netlify once purchased.

## Automatic show archiving
Events move automatically into **Past Shows** after their **end** date/time (Knoxville / America/New_York time). Flyers remain visible. For midnight sets, use the following day for `end`.

## Important notes
- Hosting, GitHub, and Pages CMS connections still require your own account authorization; they have not been created for you.
- Local opening via `file://` will not load JSON content. Preview through any local static server, e.g. `python3 -m http.server 8000` from this folder, then open `http://localhost:8000`.
- Contact form opens the visitor's mail app; it does not send server-side mail.
- Dates and venues are user supplied and not independently verified.
