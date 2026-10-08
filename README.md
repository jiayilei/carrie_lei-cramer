# Personal Homepage

A minimal, single-page personal site (sidebar + About section) modeled on the layout of felix-jimenez.com. Plain HTML and CSS, no build step.

## Customize

1. Edit `index.html`: replace every "Your Name", job title, company, email, and link.
2. Add your photo as `assets/img/avatar.png` (a square image works best).
3. Add your CV as `assets/files/CV.pdf` (or delete the CV link).
4. Optional: uncomment the Publications and News blocks in `index.html`.

## Deploy on GitHub Pages

**Option A: `username.github.io` (recommended)**

1. On GitHub, create a new public repository named exactly `<your-username>.github.io`.
2. Upload these files to the repo root (`index.html` and the `assets/` folder), or push with git:

   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```

3. In the repo, go to Settings > Pages, set Source to "Deploy from a branch", choose `main` and `/ (root)`, and save.
4. Your site will be live at `https://<your-username>.github.io` within a minute or two.

**Option B: custom domain**

After step 3, add your domain under Settings > Pages > Custom domain, then point a CNAME record (or A records) at GitHub Pages as described in GitHub's docs.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.
