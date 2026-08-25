# Lira Construction LLC — Website

A free, static one-page website for Lira Construction LLC, a family-owned custom patio cover builder serving The Woodlands, Conroe, Willis, Montgomery, Tomball, Spring, and Humble, TX. No build tools, no dependencies — plain HTML/CSS/JS.

## Structure

```
index.html          Page content
css/style.css        Styles
js/script.js         Mobile nav, footer year, contact form handler
assets/favicon.svg   Logo mark / favicon
assets/gallery/       Optimized photos + video actually used on the site
images/                Raw, full-size originals (not referenced by the site — source archive only)
```

Photos in `assets/gallery/` were cropped/resized/compressed from the originals in `images/` for fast page loads. The video (`patio-video.mp4`) was remuxed from the original `.mov` into an MP4 container for cross-browser playback — same quality, no re-encode.

## Still placeholder — fill in before launch

- Business hours (contact section) — currently `[Add your business hours]`
- Contractor license number (footer) — currently `[XXXXXX]`
- Social links in the footer (`#` placeholders)
- Testimonials — none included; add real client quotes if you have them

## Already filled in

- Phone: `(832) 897-9600`
- Email: `LiraconstructionLLC10@gmail.com`
- Service area: The Woodlands, Conroe, Willis, Montgomery, Tomball, Spring, Humble, TX
- About section (English + Spanish)
- Hero background photo, 2 before/after comparisons, 5 more project photos (including a poolside project and an in-progress framing shot), and a project walkthrough video

Send more photos any time — drop them in `images/` and they can be optimized and added to the "More Of Our Work" grid.

## Contact form

Wired up to [Formspree](https://formspree.io) (endpoint `https://formspree.io/f/meajbkok`, tied to the `LiraconstructionLLC10@gmail.com` account). Submissions go straight to that inbox as a normal email — no dashboard to check. The free Formspree plan covers 50 submissions/month; if that's ever exceeded, upgrade or swap in a different endpoint in `index.html`'s `<form action="...">`.

## Run locally

Just open `index.html` in a browser, or serve it locally:

```
npx serve .
```

## Deploy

Live at **liraconstructionllc.com**, hosted free on GitHub Pages (`Settings → Pages`, deploying from the `main` branch). The `CNAME` file in the repo root tells GitHub Pages to serve the custom domain instead of the default `gonzalezpear.github.io` URL. DNS is managed at Namecheap: 4 A records on `@` pointing to GitHub's IPs, plus a CNAME on `www` → `gonzalezpear.github.io`.

The `.nojekyll` file in the repo root tells GitHub Pages not to run Jekyll processing, which isn't needed for a plain static site.
