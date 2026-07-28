# Better Fence Tech — website

Static single-page site (HTML + videos + images, no build step). The contact form
posts to Formspree; the phone number is click-to-call.

```
index.html        the site
videos/           trimmed demo reels (no competitor logos)
images/           poster frames
robots.txt        allows crawlers, points to the sitemap
sitemap.xml       one URL for search engines
.nojekyll         tells GitHub Pages to serve everything as-is
```

## Deploy with GitHub Pages

1. Create a new repository (e.g. `betterfencetech`).
2. Upload the **contents** of this folder to the repo (drag into the GitHub web
   uploader, or `git push`).
3. **Settings → Pages → Source: Deploy from a branch → `main` / root.**
4. Add your custom domain `betterfencetech.com` under Settings → Pages → Custom domain
   (and point the domain's DNS at GitHub Pages).

## Already wired up

- **Contact form** → `https://formspree.io/f/meeynvbj` (submissions hit your inbox).
- **Phone** → 734-219-4208, click-to-call in the nav, contact section, and footer.
- **SEO** → optimized title/description, Open Graph + Twitter cards, JSON-LD
  ProfessionalService schema, canonical tag, favicon, robots.txt, and sitemap.xml.
- **Mobile** → responsive throughout; the flow graphic has a dedicated stacked
  version on phones.

## Note on absolute URLs

The SEO tags (canonical, Open Graph, sitemap) use `https://betterfencetech.com/`.
If you deploy to a different URL first (e.g. a `github.io` address), update those
values in `index.html` and `sitemap.xml` so they point at the live domain.
