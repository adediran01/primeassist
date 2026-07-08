Simple static site for PrimeAssist

How to view locally:
1. Open `site/index.html` in your browser (double-click or `file://`)

Alternatively, serve it locally with a simple HTTP server:
```bash
# from repo root
python3 -m http.server --directory site 8000
# then open http://localhost:8000
```

Quick deploy to GitHub Pages (root):
```bash
# from repo root
git checkout -b gh-pages
cp -r site/* .
git add .
git commit -m "Deploy static site"
git push origin gh-pages
# In GitHub repository settings -> Pages, set branch to gh-pages (root)
```

Or host the `site/` folder on Netlify/Vercel by dragging the folder or connecting the repo.
