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

The form on the page is front-end only — submitting it currently just shows a message and does not send an email. To make it actually work on a static site, connect it to a free form backend, e.g.:

- [Formspree](https://formspree.io) — set the form's `action` to your Formspree endpoint and change the method/JS as needed
- [Netlify Forms](https://docs.netlify.com/forms/setup/) — if hosting on Netlify, add `data-netlify="true"` to the `<form>` tag

## Run locally

Just open `index.html` in a browser, or serve it locally:

```
npx serve .
```

## Deploy to GitHub Pages (free)

1. Push this repo to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Under "Build and deployment", set **Source** to `Deploy from a branch`.
4. Choose branch `main` and folder `/ (root)`, then save.
5. Your site will be live at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

The `.nojekyll` file in the repo root tells GitHub Pages not to run Jekyll processing, which isn't needed for a plain static site.
