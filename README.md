# myportfoliov2

Sherwin Galindo — personal portfolio website. A fast, self-contained static
single-page site (HTML/CSS/JS, no build step).

## Live site (GitHub Pages)

Published at:

- **https://sherwingalindo18.github.io/myportfoliov2/**

Deployment uses GitHub Pages' **Deploy from a branch** mode:

- **Settings → Pages → Build and deployment → Source: Deploy from a branch**
- **Branch: `main` / `root`**

Because `index.html` lives at the repo root and `.nojekyll` is present, Pages
serves the site as-is (no Jekyll build). Every push to `main` republishes it.

## Custom domain

The site's SEO metadata (`sitemap.xml`, canonical + Open Graph tags) points at
`https://sherwingalindo.com`. To serve GitHub Pages from that domain, add a
`CNAME` file containing `sherwingalindo.com` and configure the domain under
**Settings → Pages → Custom domain**.

## Project structure

```
index.html              Full single-page site
css/style.css           All styles
js/main.js              Nav, animations, contact form
assets/                 profile.jpg, logo.png
og-image.png            1200x630 social share card
sherwin-galindo-cv.pdf  CV (linked from the header button)
robots.txt, sitemap.xml SEO files
.htaccess               Apache config (used only for non-Pages/Bluehost hosting)
README-DEPLOY.txt       Original Bluehost deploy notes
```

All asset paths are relative, so the site works both at a root domain and at
the `/myportfoliov2/` project path on GitHub Pages.
