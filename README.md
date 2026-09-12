# Nayem Ul Alam — Portfolio

A static portfolio site (HTML + CSS + a little JS, no build step) built from the resume content.

## Files
- `index.html` — page content
- `style.css` — all styling
- `script.js` — mobile nav toggle + footer year

## Before you deploy
Open `index.html` and replace the two placeholder contact links (in the Contact
section) with your real LinkedIn and GitHub profile URLs — the source resume
listed those as labels without links, so they need to be filled in:

```html
<li><span>LinkedIn</span><a href="#" data-placeholder="true">Add your LinkedIn URL</a></li>
<li><span>GitHub</span><a href="#" data-placeholder="true">Add your GitHub URL</a></li>
```

## Deploy on GitHub Pages
1. Create a new repository on GitHub (e.g. `portfolio`).
2. Push these three files to it:
   ```bash
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`,
   branch `main`, folder `/ (root)`, then **Save**.
5. Your site will be live at `https://<your-username>.github.io/<repo-name>/`
   within a minute or two.

## Deploy on Netlify
**Option A — drag and drop (fastest):**
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag the folder containing these three files into the browser window.
3. Netlify gives you a live URL immediately. You can rename the site
   (Site settings → Change site name) or attach a custom domain.

**Option B — connect the GitHub repo (auto-redeploys on push):**
1. Push the files to GitHub first (see steps above).
2. In Netlify, click **Add new site → Import an existing project**.
3. Pick your repository. Leave build command empty and publish directory as `.` (root).
4. Click **Deploy site**.

Both options work from the exact same files — no changes needed between them.
