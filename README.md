# PR7 Sports Club storefront

Responsive, static PR7 storefront concept with locally bundled images and fonts. Open `index.html` directly or serve the folder with any static web server. No build step or app API is required.

## Store interactions

Product sizes are selectable on product cards. The shopping bag persists product counts and sizes in browser storage, calculates a ₹79 delivery fee below ₹1,499, and applies free delivery from ₹1,499. Checkout collects delivery details in the current browser session, shows an itemized review, and opens a prefilled WhatsApp order request to PR7 at +91 73054 82605. Delivery details are not saved in browser storage. The customer must review and send the WhatsApp message to place the request.

This provides a working **order-request checkout**, not card payment processing or a server-backed order database. No payment details are collected. Payment options and availability are confirmed directly with PR7 through WhatsApp. Newsletter feedback is a local demo only.

The PR7 brand kit includes three original transparent SVG logo marks and selectable Volt, Court, and Ice accent palettes. A responsive editorial spotlight, source-noted reference imagery, branded loader, reduced-motion support, and scroll reveals are included. The palette selection and bag remain in local browser storage; checkout contact details remain in memory only.

## Vercel deployment and missing images

Deploy the **entire folder**, including `assets/`; do not upload just `index.html`. For a repository containing this project in a subfolder, set Vercel’s Root Directory to `pr7-sportsclub`. Use the **Other** framework preset and serve the project root as static files; there is no build command or build output folder for this plain HTML project. If the project itself is the repository root, use that root directly.

All storefront image, font, and logo references use relative `assets/...` paths. After deployment, open a missing asset’s path directly, for example `https://YOUR-VERCEL-DOMAIN/assets/pr7-editorial-spotlight.webp`. A 404 usually means the `assets` folder was not included in the deployment or the Vercel Root Directory points at the wrong folder. Confirm filename case exactly; Vercel runs on a case-sensitive filesystem. In browser DevTools → Network, filter by Img and inspect the failed asset’s URL and status.

## Sample-content and image rights

Product names, sizes, prices, inventory, discounts, and brand-history details are demonstration content, not a verified PR7 catalog. The selected web-reference imagery and campaign visual are documented in `assets/IMAGE-SOURCES.md`; the reference photos are not verified PR7 merchandise. Confirm usage rights and replace with approved product photography and catalog data before commercial use.
