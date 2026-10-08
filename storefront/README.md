# NTS storefront — first code milestone

Static, mobile-first storefront prototype for Not That Simple, intended for Cloudflare Pages and the existing GitHub workflow.

## Files
- `index.html` — page structure, collection, signup form, cart drawer, size guide
- `styles.css` — responsive visual system and product mockups
- `script.js` — colour selection, local cart state, quantity changes, size guide, Formspree signup

## Current functionality
- Responsive premium-minimal storefront
- System 01 product cards in Black, Off-White, White and Olive
- Current working price configured as ₹2,999 in `script.js` and markup; verify this before taking live orders
- Colour switching and add-to-bag
- Cart persists in the visitor's browser using localStorage
- Size guide using current NTS reference values; confirm fashion-line measurements against approved samples
- Early-access form posts to existing Formspree endpoint `https://formspree.io/f/xvkzawja`

## Important before real sales
This is a working **frontend milestone**, not a production-ready commerce backend. Cart contents are stored only in the visitor's browser. No orders are created, no stock is reserved, and no payments or customer accounts are processed. The checkout button intentionally explains that checkout is not connected. Do not advertise checkout as live until a secure backend and payment provider are integrated and tested.

Before launch:
1. Replace CSS tee mockups with approved product photography.
2. Confirm final price, fabric claims, size chart, shipping, returns, privacy and terms.
3. Connect backend/order storage, stock control, email notifications and chosen payment gateway.
4. Test form submission, accessibility, mobile layouts, and real checkout end-to-end.

## Deploy on Cloudflare Pages
Upload these files to the existing GitHub repository's `main` branch at the website root, preserving any existing project-specific settings. Cloudflare Pages should redeploy automatically. If the current landing page uses a separate repo/path, merge these files into that same published root rather than creating a second project.
