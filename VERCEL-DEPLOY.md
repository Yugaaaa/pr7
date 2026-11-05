# Vercel static deployment — PR7 storefront

The PR7 site is plain static HTML/CSS/JavaScript. Its images, SVG logos, and fonts live in the sibling `assets/` directory and are referenced with relative paths.

## Deploy this project

Deploy the complete `pr7-sportsclub` folder, not a copied `index.html` alone. In Vercel, select the project folder as **Root Directory** (choose `pr7-sportsclub` when it is a subfolder in a larger repository), use the **Other** framework preset, and leave build command and output directory unset for this no-build static project. `index.html`, `styles.css`, `app.js`, and `assets/` should all sit together at the selected root.

## Verify image delivery

After redeploying, open these paths on the deployed host:

- `/assets/pr7-editorial-spotlight.webp`
- `/assets/community-reference.jpg`
- `/assets/pr7-wordmark.svg`

They should return the image themselves, not the homepage. If they return 404, check that the entire `assets/` directory was committed/uploaded and that the Vercel Root Directory points to this project folder. Paths are case-sensitive. In browser DevTools → Network, filter by Img and inspect the exact failed URL/status. If an image URL returns 200 but remains invisible, check the browser Console for CSS or Content-Security-Policy errors.

The ZIP archive preserves the full static project folder structure for redeployment.
