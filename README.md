# myportfoliov2

Sherwin Galindo — personal portfolio website. A fast, self-contained static
single-page site (HTML/CSS/JS, no build step).

## Live site (GitHub Pages)

This repo auto-deploys to **GitHub Pages** via
[`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml).

Once the workflow has run on the default branch, the site is published at:

- **https://sherwingalindo18.github.io/myportfoliov2/**

The workflow enables Pages automatically (`configure-pages` with
`enablement: true`) and publishes the repository root. It runs on every push to
`main` and can also be triggered manually from the **Actions** tab
(*Run workflow*).

> If the first run is blocked, open **Settings → Pages** and set the source to
> **GitHub Actions**, then re-run the workflow.

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
