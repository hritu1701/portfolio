# Hritu Raj — Portfolio

A single-page 3D portfolio (WebGL orb + particles, smooth scroll, kinetic type).
Pure static: one `index.html`, no build step, all libraries from CDN.

## Run locally
Just open `index.html` in a browser, or serve it:
```bash
python3 -m http.server 8080   # then visit http://localhost:8080
```

## Deploy on Render (Static Site)

**Option A — from the dashboard**
1. Push this folder to a GitHub repo.
2. Render → **New** → **Static Site** → connect the repo.
3. Settings:
   - **Build Command:** *(leave empty)*
   - **Publish Directory:** `.`
4. **Create Static Site** → Render serves it on a free `*.onrender.com` URL.

**Option B — Blueprint**
The included `render.yaml` defines the static site. In Render choose **New → Blueprint**,
point it at the repo, and it configures everything automatically.

## Customize
- Colors / fonts: the `:root` block at the top of `index.html`.
- Copy, projects, links: the HTML sections (`#about`, `#work`, `#projects`, `#contact`).
- The 3D orb shader + particles live in the `<script>` at the bottom.

## Quick push
```bash
cd portfolio
git init
git add .
git commit -m "Hritu Raj portfolio"
git branch -M main
git remote add origin https://github.com/hritu1701/portfolio.git
git push -u origin main
```
