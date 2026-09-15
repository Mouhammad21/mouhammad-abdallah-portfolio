# Mouhammad Abdullah — Performance Marketing Manager Portfolio

A single-page portfolio built for job applications: About, Specialties,
Experience, Certifications, Tools, Track Record, Contact. Plain HTML/CSS/JS —
no build step, so it works directly on GitHub Pages.

## Before you publish — one thing left

- **Your photo** — add a file named exactly `profile.jpg` to this folder
  (same folder as `index.html`). It's already wired into the header and hero
  with a graceful "MA" initials fallback if the file is missing, so the site
  looks fine either way — but a real photo is a big trust signal for
  recruiters.

Everything else (contact info, experience, theme colors) is filled in with
real content.

## Publish it on GitHub Pages

You've already got this set up and live — just repeat the same git commands
whenever you update these files:

```bash
git add .
git commit -m "Update portfolio"
git push
```

GitHub Pages rebuilds automatically within a minute or two of every push.

## Making the contact section actually receive messages

This is a static site, so Contact currently just links out to `mailto:` /
`tel:` / LinkedIn. For a working on-page form later, the simplest options are
[Formspree](https://formspree.io) or [Getform](https://getform.io) — both
work with a plain HTML `<form>` on the free tier, no backend required.
