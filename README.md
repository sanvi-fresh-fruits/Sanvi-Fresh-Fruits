# Saanvi Fresh Fruits — Landing Page

Single-page static website. No build step, works directly on GitHub Pages.

## Files

```
index.html               the whole page (HTML + CSS + JS)
assets/saanvi-logo.png    main logo (hero)
assets/saanvi-logo-sm.png small logo (header, footer)
assets/favicon.png        browser tab icon
.nojekyll                 tells GitHub Pages to serve files as-is
```

## Before going live: update business details

Open `index.html`, find this block near the bottom, and replace the sample values:

```js
const BUSINESS = {
  phone:    "+91 98765 43210",      // shown on the page
  whatsapp: "919876543210",         // country code + number, digits only
  email:    "orders@saanvifreshfruits.com",
  address:  "Shop address, City, State",
  hours:    "Mon to Sun, 6:00 am to 9:00 pm"
};
```

Every WhatsApp button, the phone/email links, the address and the timings update from here.

The season calendar is in the `SEASONS` list in the same script, if months need adjusting.

## Publish on GitHub Pages

1. Create a new repository (for example `saanvi-fresh-fruits`).
2. Upload all files from this folder, keeping the `assets` folder as is.
3. Go to **Settings → Pages**, set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. The site will be live at `https://<username>.github.io/saanvi-fresh-fruits/` in a minute or two.

For a custom domain, add it under **Settings → Pages → Custom domain** and point the domain's DNS to GitHub Pages.
