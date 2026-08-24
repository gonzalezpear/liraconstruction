# Lira Construction — Website

A free, static one-page website for Lira Construction (general contracting & residential remodeling). No build tools, no dependencies — plain HTML/CSS/JS.

## Structure

```
index.html        Page content
css/style.css      Styles
js/script.js       Mobile nav, footer year, contact form handler
assets/favicon.svg Logo mark / favicon
```

## Before launch — replace placeholders

Search the project for these and fill in real values:

- Phone number: `(555) 555-5555`
- Email: `info@liraconstruction.com`
- Service area / city: `[City, State]`
- Contractor license number: `[XXXXXX]`
- Social links in the footer (`#` placeholders)
- Project photos in the "Recent Projects" section (currently placeholder tiles)
- Testimonials — none included; add real client quotes if you have them

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
