# PR7 Sports Club storefront

A responsive, static storefront prototype rebranded for PR7 Sports Club. The visual direction uses a charcoal base, sharp lime accents, locally bundled condensed display and clean body fonts, and athletic editorial imagery. A glassmorphism APEX product spotlight adds a thumbnail carousel, selectable sizes and colors, and a local add-to-bag action.

## Run locally

Open `index.html` directly in a modern browser, or serve this folder with any static file server. There is no build step and no package installation required.

## Included interactions

- Category filters, price sorting, and local product search
- Saved products and a shopping bag persisted in browser `localStorage`
- Responsive mobile navigation and bag drawer
- Newsletter form feedback kept entirely in the browser
- An animated editorial spotlight using a generated local image and bundled fonts
- A branded opening loader that respects reduced-motion preferences
- Footer shortcuts for the supplied Instagram profile, map location, and phone number

This is frontend-only sample storefront code. Product names, pricing, imagery, brand details, and the 2024 brand-establishment date are demo content and should be replaced with approved PR7 materials. The bag is not connected to checkout, inventory, payment, email collection, or any server. The page makes no app API calls and is not deployed or hosted by Manus.

## Files

- `index.html` — page structure and accessible controls
- `styles.css` — responsive styling and design tokens
- `app.js` — local-only UI behavior and sample product catalog
- `assets/` — locally stored editorial imagery and font files
