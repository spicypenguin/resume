# resume.jeffable.com

Jeff Sinclair's resume site. Plain static HTML/CSS/JS — no build step, no framework, no theme dependency.

## Structure

- `index.html` — the whole site
- `assets/css/style.css` — styles, including a dedicated `@media print` stylesheet for the "Save as PDF" button
- `assets/js/main.js` — wires up the "Save as PDF" button (triggers the browser print dialog; choose "Save as PDF" as the destination)
- `assets/images/profile.jpg` — headshot

## Local preview

Any static file server works, e.g.:

```
npx serve .
```

## Deployment

This is a plain static site — point any static host (Vercel, Netlify, GitHub Pages, etc.) at the repo root with no build command and no output directory override needed. If the previous host (e.g. Vercel/Aerobatic) is still configured to run a Hugo build, switch its framework preset to "Other" / static.

## Editing content

There's no CMS or templating — edit `index.html` directly. Sections are in DOM order: hero, profile, skills, experience (grouped by company), education, footer.

Three bullet lists under the Stripe roles in the Experience section are marked with a "Draft — please edit" flag and an HTML comment above them — replace those with real specifics before sending this resume out.
