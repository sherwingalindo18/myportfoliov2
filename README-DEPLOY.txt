SHERWINGALINDO.COM — REDESIGN DEPLOY NOTES
==========================================

WHAT'S INSIDE
  index.html                 The full site (single page)
  css/style.css              All styles
  js/main.js                 Nav, animations, contact form
  sherwin-galindo-cv.pdf     Your CV (linked from the header button)
  robots.txt, sitemap.xml    SEO files
  .htaccess                  HTTPS redirect + caching + compression
  assets/                    << PUT YOUR IMAGES HERE (see below)

IMAGES — ALREADY INCLUDED
  assets/profile.jpg  — your photo (hero + about + CV)
  assets/logo.png     — square logo generated from your photo
  og-image.png        — 1200x630 social share card (branded, with photo)
  Replace any of them anytime by uploading a new file with the same name.

UPLOAD TO BLUEHOST
  1. cPanel > File Manager > public_html (for sherwingalindo.com)
  2. Back up / delete the old site files
  3. Upload ALL files in this folder, keeping the folder structure
     (css/, js/, assets/ must stay as folders). Include .htaccess —
     enable "Show hidden files" in File Manager settings to see it.
  4. Visit https://sherwingalindo.com and hard-refresh (Ctrl+Shift+R)

ADDING PORTFOLIO LINKS
  In index.html, find the "WORK" section. Each project card is an <a>.
  Change href="#" to the live URL, add target="_blank" rel="noopener",
  and remove aria-disabled="true" and tabindex="-1".

CONTACT FORM
  The form opens the visitor's email app pre-filled (works on static
  hosting with no backend). If you later want direct-to-inbox delivery,
  a service like FormSubmit or Formspree can be wired to the same form.

UPDATING THE CV
  Replace sherwin-galindo-cv.pdf with any newer version using the same
  filename — the header button will keep working.
