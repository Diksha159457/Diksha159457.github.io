# Portfolio — deploy & update

Two files, no build step: `index.html` and `covid-dashboard.webp`.

## Deploy (GitHub Pages, free)

1. Create a public repo named `Diksha159457.github.io`.
2. Upload `index.html` and `covid-dashboard.webp` to the repo root (add `resume.pdf` too, see below).
3. Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/root`.
4. Site goes live at `https://diksha159457.github.io/` within a minute or two.
5. Link-preview metadata already points at `https://diksha159457.github.io/`; update it if you move to a custom domain.

Vercel / Netlify also work: drag the folder onto their dashboard; no settings needed.

## Add your résumé

1. Put `resume.pdf` next to `index.html`.
2. Near the bottom of `index.html`, set `var RESUME_URL = "resume.pdf";`
3. The "Download résumé" buttons appear automatically; until then visitors see "Request résumé".

## Update content

Everything is plain HTML, grouped by comment banners (`<!-- ============ WORK ============ -->` etc.):

- **A project:** copy one `<article class="project">` block inside WORK and edit the text, stack tags and links. Keep claims to what the repo shows.
- **A smaller project:** copy an `<article>` inside MORE WORK.
- **Skills:** edit the `.matrix` blocks in SKILLS.
- **Experience / certificates:** add an `<li>` to the `.timeline` list in EXPERIENCE (newest first).
- **Availability:** edit the badge text in HERO and the paragraph in CONTACT; delete the `<span class="status">` line when you're not looking.
- **Email / links:** search-and-replace `dikshashahi299@gmail.com`, `diksha-shahi`, `Diksha159457`.

Colours and fonts are tokens at the top of the `<style>` block (`--signal` is the cyan accent).
