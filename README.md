# The Cake Shop Template

A ready-to-use, one-page website template for bakeries and cake shops. Showcase your products, share your location and hours, and give customers a clear way to order—all in a clean, professional design.

This template is built for speed and simplicity. It loads fast, looks great on phones, and uses clean HTML that search engines love. Just swap in your business info and images, and you're ready to go live.

## Why Use This Template?

- ⚡ **Lightweight** — Minimal code, fast load times
- 🎂 **Product-first design** — Your cakes take center stage
- 📱 **Mobile-first** — Looks great from phones to desktops
- ♿ **Semantic HTML** — Accessible and SEO-friendly
- ✨ **Smooth animations** — Subtle scroll reveal effects
- 🎨 **Easy to customize** — All your info in one file

## What's Included

| Section | Description |
|---------|-------------|
| **Header** | Sticky navigation with your shop name and "Order Now" button |
| **Hero** | Large tagline, call-to-action buttons, contact info, featured image |
| **Top Cakes** | Grid of your 6 best-selling products with photos and prices |
| **About** | Brief description of your bakery |
| **Hours & Location** | Business hours and address in card format |
| **Order** | Clear call-to-action with phone number |
| **Footer** | Copyright and attribution |

## Customize Your Template

All your business information lives in one file: `src/pages/index.astro`

### Business Information

Edit the `shop` object:

```javascript
const shop = {
  name: "The Cake Shop",                    // Your business name
  tagline: "Fresh cakes, ready for...",     // Your main headline
  ctaPrimary: { label: "Order Now", href: "#order" },
  ctaSecondary: { label: "View Top Cakes", href: "#top-cakes" },
  phone: "(555) 555-5555",                  // Your phone number
  address: "123 Sweet St, Long Beach, CA",  // Your address
  hours: "Mon–Sat 9am–6pm · Sun 10am–4pm", // Your hours
};
```

### Products

Edit the `topCakes` array:

```javascript
const topCakes = [
  {
    name: "Assorted Dozen Sponge Cakes",  // Product name
    price: "$29.99",                       // Price
    note: "Best seller",                   // Short description
    img: "/img/your-image.webp"            // Image path
  },
  // ... add up to 6 products
];
```

### Images

Replace images in the `public/img/` folder:

| Image | Location | Recommended Size |
|-------|----------|------------------|
| Hero image | Used in hero section | 4:3 aspect ratio (e.g., 800×600px) |
| Product images | Used in product cards | 4:3 aspect ratio (e.g., 400×300px) |

**Tips:**
- Use `.webp` format for best performance
- Keep file sizes under 200KB
- Use descriptive filenames

### Navigation Links

Edit the `navLinks` array if you change section IDs:

```javascript
const navLinks = [
  { label: "Top cakes", href: "#top-cakes" },
  { label: "About", href: "#about" },
  { label: "Hours", href: "#hours" },
  { label: "Order", href: "#order" },
];
```

## Build (Optional)

If you want to modify the template and rebuild:

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

The production files will be in the `dist/` folder.

## Deploy to GitHub Pages

### Option 1: Use the Static Files Directly

If you received the pre-built static files:

1. Create a new GitHub repository
2. Upload all files from the `dist/` folder to the repository root
3. Add an empty `.nojekyll` file to the repository root
4. Go to **Settings** → **Pages**
5. Under "Source", select **Deploy from a branch**
6. Choose the **main** branch and **/ (root)** folder
7. Click **Save**

Your site will be live at `https://yourusername.github.io/your-repo-name/`

### Option 2: Build and Deploy

If you have the source files and Node.js installed:

1. Run `npm run build` to generate the `dist/` folder
2. Follow Option 1 steps to upload the `dist/` contents

## License

This template is **free for personal and commercial use**, including client projects.

**One requirement:** Keep the attribution link in the footer that links to [PixuVault](https://pixuvault.com/).

See [LICENSE.md](LICENSE.md) for full terms.

---

## VERSION_LOG

### v0.1.0 — 2026-01-17

- Initial release: product-first cake shop template
- Scroll reveal animations on sections and product cards
- Responsive design (mobile-first)
- Semantic HTML structure
- Pattern-based component architecture
