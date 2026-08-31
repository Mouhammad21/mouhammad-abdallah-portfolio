# Mouhammad — Performance Marketing Manager Portfolio

A single-page portfolio site: About, Specialties, Experience, Certificates,
Tools, Track Record, Contact. Plain HTML/CSS/JS — no build step, so it works
directly on GitHub Pages.

## Before you publish — fill these in

Most content is now pulled from your real LinkedIn profile (experience,
certifications, tools, results). Only a few placeholders are left — search
`index.html` for square brackets `[...]`:

- **Experience** — `[Add start date]` for Clickvertise (LinkedIn doesn't list
  it as a formal role, so add the year you actually founded it)
- **Contact** — your real email and phone/WhatsApp number (LinkedIn doesn't
  expose these to automated tools, so they need to be typed in manually)
- Optional: add a headshot/photo, and add metrics to the other **Track
  record** case studies (Twister Technologies, Index Properties, etc.) for
  any results you're able to share publicly

## Publish it on GitHub Pages (username.github.io)

1. Create a new repository on GitHub. For a root domain like
   `yourusername.github.io`, name the repo exactly `yourusername.github.io`.
   For a project site, any repo name works and it'll publish at
   `yourusername.github.io/repo-name`.
2. Push these three files (`index.html`, `style.css`, `script.js`) to the
   repo's default branch:
   ```bash
   git init
   git add .
   git commit -m "Launch portfolio site"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**, set **Source** to "Deploy from a
   branch", branch `main`, folder `/ (root)`, then **Save**.
4. GitHub gives you a live URL in a minute or two — usually
   `https://yourusername.github.io/`.

## Optional: custom domain

If you own a domain and want it instead of the github.io address:

1. Add a `CNAME` file to the repo root containing just your domain, e.g.
   `yourdomain.com`.
2. At your domain registrar, point it at GitHub Pages: an `A` record to
   GitHub's IPs (185.199.108.153, .109.153, .110.153, .111.153) for a root
   domain, or a `CNAME` record to `yourusername.github.io` for a subdomain.
3. Back in **Settings → Pages**, enter the custom domain and enable
   **Enforce HTTPS** once it verifies.

## Making the contact section actually receive messages

This is a static site, so the Contact section currently just links out to
`mailto:` / `tel:` / LinkedIn. If you want a working on-page form later, the
simplest options are [Formspree](https://formspree.io) or
[Getform](https://getform.io) — both work with a plain HTML `<form>` and
free-tier, no backend required.
