# The Cake Shop Template

A ready-to-use, one-page website template for bakeries and cake shops. Showcase your products, share your location and hours, and give customers a clear way to order — all in a clean, professional layout.

This repo contains only **static files** (HTML/CSS/images). You can edit it directly and deploy it with GitHub Pages.

## Why use this template?

- Lightweight and fast
- Product-first layout (your items are the focus)
- Mobile-first responsive design
- Semantic HTML (accessibility + SEO-friendly)
- Subtle scroll-reveal animation (small “wow” without being distracting)
- Easy to edit (mostly one file)

## What’s included

- Sticky header with nav + “Order Now” CTA
- Hero section with headline + featured image
- Top products grid (6 items)
- About section
- Hours & location cards
- Order CTA section
- Footer with required attribution link

## Customize (the simple way)

You will mostly edit:

- `index.html` (text, links, product names/prices)
- `img/` (replace images)
- `index.css` (optional styling changes)

### 1) Change business info
Open `index.html` and edit:
- Shop name (header + footer)
- Hero headline + subtext
- Phone number + address
- Hours text

Tip: use your editor search (Ctrl+F) for:
- `The Cake Shop`
- `(555)`
- `123 Sweet St`
- `Long Beach bakery`

### 2) Replace images
Put your images into `img/` and update the `<img src="img/your-file.webp">` paths in `index.html`.

Recommended:
- Hero image: 4:3 aspect ratio (ex: 800×600)
- Product images: 4:3 aspect ratio (ex: 400×300)
- Use `.webp` if possible; keep files reasonably small.

### 3) Update products (6 items)
In `index.html`, find the “Top cakes” section and edit:
- product name
- price
- short note
- image filename

## Deploy to GitHub Pages

1. Go to **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: **main**
4. Folder: **/ (root)**
5. Save

Your site will be live at:
`https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

## License (attribution required)

Free for personal and commercial use, including client work.

One requirement: keep the PixuVault attribution link on the homepage.
See `LICENSE.md`.

---

## VERSION_LOG

### v0.1.0 — 2026-01-17
- Initial release: product-first cake shop template
- Flattened output: `index.html` + `index.css` + `img/`
- Subtle scroll reveal on sections
