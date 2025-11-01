# Sahara Brass Industries — Static Website

Simple static website for Sahara Brass Industries. This repo contains plain HTML/CSS/JS files and static assets in the `static/` folder.

Quick links to main pages in this repo:
- [`index.html`](index.html)
- [`about.html`](about.html)
- [`products.html`](products.html)
- [`contact.html`](contact.html)
- [`menubar.html`](menubar.html)
- [`footer.html`](footer.html)

Features
- Responsive static site built with Tailwind CSS (CDN).
- Lightweight animations using GSAP + ScrollTrigger.
- Product gallery with filtering and animations in [`products.html`](products.html).
- Reusable navbar & footer loaded via JS partials: [`menubar.html`](menubar.html) and [`footer.html`](footer.html).
- Static assets under `static/` (images, logos, product photos).

Run locally
1. Open the site directly in a browser:
   - Open `index.html` in your browser.
2. Recommended: use VS Code + Live Server extension for a dev server.
   - The workspace config uses port 5501: see [.vscode/settings.json](.vscode/settings.json).
   - Start Live Server (or run `Live Server: Open with Live Server`) and open http://127.0.0.1:5501/.

Push to GitHub
1. Initialize and push:
```sh
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```
2. (Optional) If you want to host the site on GitHub Pages automatically, add the workflow included in `.github/workflows/deploy.yml` (already added here). The workflow builds (no build step needed for static files) and deploys the repository root to GitHub Pages.

GitHub Pages (automatic deploy)
- The provided GitHub Actions workflow uploads the repository root as the Pages artifact and deploys it.
- After pushing, enable Pages in your repository Settings → Pages (the action will publish the site).

Notes
- Update any image paths inside `static/` if you add/rename assets.
- The enquiry modal in [`footer.html`](footer.html) is a client-side prototype; integrate your backend/email service for production use.
- License: add your preferred license file (e.g., `LICENSE`) if needed.

Maintainers
- Developed by Rumit Vasoya (credit in footer).