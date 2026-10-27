# Spice Garden - QR Ordering Demo

Frontend-only demo. All data is stored in the browser (localStorage). No backend or database.

## How to demo
1. Open `/menu?table=4` in one browser tab (customer view).
2. Open `/admin` in another tab of the SAME browser. Login: admin / demo123.
3. Place an order in the first tab. It appears instantly on the dashboard. Change its status and watch the customer's order page update.

## Run locally
Use any static server, for example: `npx serve -s .` (the `-s` flag enables the /menu and /admin routes).

## Deploy (Cloudflare Pages)
Upload this folder. The `_redirects` file routes every path to index.html. Then open Admin > Tables & QR and set the Base URL to your live domain before printing QR codes.

## Food images
Put images in `assets/` using the file names below (JPG), or paste image URLs in Admin > Menu.
paneer-tikka, french-fries, veg-sandwich, paneer-butter-masala, kadai-paneer, dal-tadka, mix-veg, butter-naan, tandoori-roti, jeera-rice, veg-biryani, masala-dosa, hakka-noodles, sweet-lassi, masala-chaas, cold-drink, gulab-jamun, ice-cream

## Customise
Hotel name, tagline, table count, currency and demo login are in the CFG object at the top of the script in index.html.
