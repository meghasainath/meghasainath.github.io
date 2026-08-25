# Megha Sainath — Portfolio

A three-page static portfolio site (Home · Experience · Interests), built as plain
HTML/CSS with no build step. Designed to be hosted for free on **GitHub Pages**.

```
index.html          # Home — intro, education, work, contact
experience.html     # Selected work + resume link
interests.html      # Books + photography
assets/             # Portrait + photographs (referenced by the pages)
.nojekyll           # Tells GitHub Pages to serve files as-is
```

## Publishing to GitHub Pages (megha's own account)

> Replace `USERNAME` below with Megha's actual GitHub username.

### Option A — user site at `https://USERNAME.github.io`
1. On github.com, signed in as Megha, create a **new public repository** named
   exactly **`USERNAME.github.io`**. Do not add a README (this repo already has one).
2. From this folder, push it up:
   ```bash
   git init            # (already done if this was set up for you)
   git add -A
   git commit -m "Publish portfolio"
   git branch -M main
   git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**. Under "Build and deployment", set
   Source = **Deploy from a branch**, Branch = **main / (root)**, then Save.
4. Wait ~1 minute. The site goes live at **https://USERNAME.github.io**.

### Option B — no command line (web upload)
1. Create the public repo `USERNAME.github.io` as above.
2. Click **Add file → Upload files**, drag in `index.html`, `experience.html`,
   `interests.html`, the `assets/` folder, and `.nojekyll`, then **Commit**.
3. Enable Pages under **Settings → Pages** (Branch = main / root) as in Option A.

## Editing later
- Text lives directly in the `.html` files — open and edit, no tools needed.
- To swap a photo, replace the matching file in `assets/` (keep the same name),
  or add a new `<img src="assets/…">` inside the `.photo-grid` in `interests.html`.
