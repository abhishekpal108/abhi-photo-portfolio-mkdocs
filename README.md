# Abhi Photography — MkDocs Portfolio (Free, GitHub Pages)

A free, Python-powered static portfolio for photography. Built with **MkDocs + Material** with a lightbox gallery.

## 🚀 Quick Start (Local Preview)

1. Install Python 3.10+
2. Create a virtualenv (recommended)
3. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```
4. Run local server:
   ```bash
   mkdocs serve
   ```
   Visit http://127.0.0.1:8000

## 🌐 Deploy to GitHub Pages (Free)

1. Create a **public** GitHub repo named `abhi-photo-portfolio-mkdocs` (or any name).
2. Push this project to your repo:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Abhi photo portfolio (MkDocs)"
   git branch -M main
   git remote add origin https://github.com/<your-github-username>/<your-repo>.git
   git push -u origin main
   ```
3. GitHub Actions will auto-deploy to the `gh-pages` branch.  
   If it doesn't exist yet, push and then check **Actions** tab for the workflow run.
4. In **Settings → Pages**, set **Source: Deploy from a branch** and select `gh-pages` / `/ (root)`.
5. Your site will be live at: `https://<your-github-username>.github.io/<your-repo>/`

> Update `site_url` in `mkdocs.yml` to your final URL.

## 🖼 Add Photos

Put web-optimized JPG/PNG images into `docs/photos/<category>/`.  
Then reference them in the relevant Markdown in `docs/gallery/*.md` using the `.glightbox` class, e.g.:

```markdown
![Misty woods](../photos/nature/sample1.jpg){ .glightbox data-gallery="nature" }
```

Repeat for each image. The lightbox lets users click-to-zoom and swipe.

## 🧭 Customize

- Edit `mkdocs.yml` for site name, colors, and navigation.
- Edit `docs/index.md`, `docs/about.md`, and `docs/contact.md`.
- Add/rename gallery categories by creating new Markdown files in `docs/gallery/` and folders in `docs/photos/`.

## 🔒 Privacy & Performance Tips

- Export photos around **1200–1600px wide** for faster loads.
- Strip EXIF if you don’t want metadata shared.
- Avoid huge galleries on a single page; split by category.

## 🧰 Tech

- Python, MkDocs, Material for MkDocs
- Plugins: glightbox, minify, search
- Deploy: GitHub Actions → GitHub Pages (free)
```

#requirements
