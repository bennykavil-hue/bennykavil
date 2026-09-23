# Benny Antony K — Professional Profile

A single-page, mobile-responsive profile site for Benny Antony K: IT professional since 1986, offering IT services, digital solutions, and online software training.

## Files

- `index.html` — the complete page (HTML, CSS, and fonts all self-contained in one file, aside from Google Fonts loaded over the network).

## Viewing it

Just open `index.html` in any browser — no build step or server required. To publish it, upload it as-is to any static host (GitHub Pages, Netlify, your own web server, etc.) as the site's home page.

## Structure

The page is one HTML file with an embedded `<style>` block, organized into sections in this order:

1. **Header / nav** — sticky top bar with jump links to each section below.
2. **Hero** — name, role, and a one-line pitch.
3. **About** (`#about`) — background and experience summary.
4. **Skills** (`#skills`) — tag list of technical skills.
5. **Education** (`#education`) — timeline of qualifications.
6. **Projects** (`#projects`) — cards for each project, each linking out to the live site.
7. **Contact** (`#contact`) — availability note, email, and phone.
8. **Footer** — copyright line.

## Design notes

- **Fonts:** Fraunces (headings), IBM Plex Sans (body text), IBM Plex Mono (small labels, dates, tags) — loaded from Google Fonts via `<link>` tags in `<head>`.
- **Colors:** defined as CSS custom properties at the top of the `<style>` block (`--navy`, `--paper`, `--teal`, `--amber`, `--ink`, `--muted`, `--line`), so the palette can be changed in one place.
- **Responsive:** built mobile-first with fluid type (`clamp()`), flex-wrapping nav and skill tags, and a breakpoint at `480px` for tighter spacing on small phones.

## Making common edits

- **Add a new skill:** duplicate a `<span class="skill-tag">...</span>` line inside `#skills`.
- **Add a new project:** duplicate a `<div class="project">...</div>` block inside `#projects`, update the heading, link, and description.
- **Add an education entry:** duplicate an `<li>` block inside the `<ul class="timeline">` in `#education`.
- **Update contact details:** edit the `mailto:` and `tel:` links inside `#contact`.
- **Change colors:** edit the values in the `:root { ... }` block near the top of the `<style>` section.
