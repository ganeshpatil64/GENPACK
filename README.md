# GENPACK
 
A minimalist, black-and-white e-commerce storefront concept — inspired by the everyday experience of shopping online, but built from scratch with its own visual identity. GENPACK is a static, front-end-only demo: no backend, no database, everything runs in the browser.
 
**Live demo:** https://genpack-snowy.vercel.app
 
## What this is
 
GENPACK is a single self-contained web page (HTML, CSS, and JavaScript all in one file) that simulates a full shopping experience:
 
- Browse a catalogue of 16 products across five categories
- Filter by category and search by product name, live
- Add items to a cart, adjust quantities, remove items
- See a running subtotal, shipping cost, and total update in real time
- Log in or sign up through a modal with basic form validation
- Complete a mock checkout once logged in
There is no server, no real payment processing, and no data storage between visits — refreshing the page resets the cart and login state. It's meant as a front-end demo and a starting point, not a production store.
 
## Design
 
The whole interface is built around a strict black-and-white palette, with product cards inverting to black on hover as the page's one signature visual moment. Product images are hand-drawn inline SVG icons (no external image files or stock photos), so the page loads instantly and works offline once downloaded. Typography pairs Space Grotesk (headings) with Inter (body text).
 
## Tech stack
 
- Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build step, no dependencies to install
- Google Fonts loaded via CDN for typography
- All application state (cart contents, logged-in user) lives in memory only, using plain JavaScript variables — nothing is written to local storage or a database
## Project structure
 
```
genpack/
└── index.html   ← the entire site: markup, styles, and logic in one file
```
 
## Running locally
 
Since there's no build process, you can open `index.html` directly in any browser, or serve it with any static file server, for example:
 
```bash
npx serve genpack
```
 
## Deployment
 
This project is deployed on [Vercel](https://vercel.com) as a static site:
 
- **Framework preset:** Other (no framework, no build step)
- **Root directory:** `genpack`
- **Build command / Output directory:** left blank — the file is served as-is
- **Environment variables:** none required
Live at: **https://genpack-snowy.vercel.app**
 
## Notes
 
This is a demo storefront built for practice/portfolio purposes. It is not affiliated with any real retail brand, and product listings, prices, and reviews are placeholder content.
 