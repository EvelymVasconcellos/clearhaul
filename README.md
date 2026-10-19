# CLEARHAUL — Concept Project

Fictional junk removal brand. Concept site designed and developed by EV to demonstrate UX/UI design,
frontend development, motion design and real-time 3D.

**CLEARHAUL is a fictional brand.** Contact details are illustrative and the quote form is a demo:
it does not send or store any data.

## Stack
- Single static page: HTML, CSS and vanilla JavaScript (no build step)
- Three.js 0.160 (procedural 3D truck and trailer) and GSAP 3.12.5 + ScrollTrigger, loaded from public CDNs
- Bilingual EN-US / PT-BR: strings in `i18n/en.json` and `i18n/pt-BR.json`, choice saved in localStorage

## Structure
```
index.html        page, styles and scripts
i18n/en.json      English (default)
i18n/pt-BR.json   Brazilian Portuguese
_headers          Cloudflare Pages response headers
```

## Run locally
The translation files load with `fetch`, so serve the folder over HTTP:
```
python3 -m http.server 8080
```
then open http://localhost:8080.

## Deploy (Cloudflare Pages)
Connect this repository in Cloudflare Pages with:
- Framework preset: None
- Build command: (empty)
- Build output directory: `/`
