# ThreadDesk Website

Static website for [ThreadDesk](https://threaddesk.com) — alteration shop management software for solo seamstresses.

## Hosting on GitHub Pages

1. Push this folder to a GitHub repository (e.g. `threaddesk/threaddesk.github.io`)
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch → main → / (root)**
4. Your site will be live at `https://[username].github.io` or your custom domain

## Custom Domain Setup

1. In GitHub Pages settings, add your custom domain: `threaddesk.com`
2. Add a `CNAME` record in your DNS pointing to `[username].github.io`
3. Enable **Enforce HTTPS** once the domain is verified

## File Structure

```
threaddesk/
├── index.html          ← Homepage (main landing page)
├── about.html          ← About / our story
├── contact.html        ← Contact form + get started
├── faq.html            ← FAQ with accordion
├── privacy.html        ← Privacy policy
├── terms.html          ← Terms of service
├── sitemap.xml         ← SEO sitemap
├── robots.txt          ← Search engine instructions
├── css/
│   └── style.css       ← All styles (shared across pages)
└── js/
    └── main.js         ← Navigation, scroll reveal, form handling
```

## Before Launching

- [ ] Replace `YOUR_FORM_ID` in `contact.html` with your real [Formspree](https://formspree.io) form ID
- [ ] Update `sitemap.xml` with your real domain
- [ ] Update `robots.txt` sitemap URL with your real domain
- [ ] Update all `https://threaddesk.com` references if using a different domain
- [ ] Add Google Analytics or Plausible tracking script if desired
- [ ] Register ThreadDesk with Google Search Console and submit `sitemap.xml`

## SEO Notes

The site includes:
- Semantic HTML with proper heading hierarchy
- Meta descriptions on every page
- Open Graph tags on homepage
- JSON-LD structured data (SoftwareApplication schema on homepage, FAQPage on faq.html)
- XML sitemap
- robots.txt
- Canonical URLs on all pages
- Alt text on all images
- Mobile-responsive layout

## Design System

Colors are defined as CSS variables in `style.css`:
- `--ink` — dark brown-black (primary)
- `--cream` — warm off-white (background)
- `--gold` — Charleston gold (accent)
- `--sage` — sage green (success/badges)

Fonts: Cormorant Garamond (display) + DM Sans (body) via Google Fonts
