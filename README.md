# Malena Ronquetti: personal website

A static one-page site (`index.html` + `style.css`), no build step. It follows the visitor's light/dark preference and has a toggle in the header.

## Publish on GitHub Pages

1. Create a GitHub account if you don't have one, then make a **new public repository** named exactly `<your-username>.github.io`.
   That name gives you the address `https://<your-username>.github.io`.
2. Upload the files: on the new repo page click **uploading an existing file**, drag in `index.html`, `style.css` and this `README.md`, then **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment*, set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. Wait a minute or two and open `https://<your-username>.github.io`.

Or from a terminal in this folder:

```bash
git init -b main
git add .
git commit -m "First version of my website"
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```

## Editing

- All content is in `index.html`, one commented block per section (HERO, ABOUT, EXPERIENCE…).
- Colours are variables at the top of `style.css` (`--accent` is the teal).
- The page has a Content Security Policy (`<meta http-equiv="Content-Security-Policy">` in `index.html`). If you add scripts or load files from another site, allow them there.
