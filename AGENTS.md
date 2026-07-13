# Codex Project Context

## Project
- Static website for Dra. Mayra Valois, a dentist in Cali, Colombia.
- Public domain/canonical URL used in metadata: `https://mayravalois.com/`.
- The site focuses on aesthetic and functional dentistry, service pages, success cases, contact, and local SEO.

## Stack And Structure
- Static HTML/CSS/JavaScript. Do not add a framework unless the user explicitly asks.
- Main page: `index.html`.
- Service pages: `servicios/*/index.html`.
- Main stylesheet: `assets/css/styles.css`.
- Images and local visual assets: `assets/img/`.
- SEO crawl files: `robots.txt` and `sitemap.xml`.

## Current Site Conventions
- Language is Spanish for Colombia (`es_CO` metadata is used).
- Visual style is premium clinical: dark background, gold accents, serif display typography, elegant spacing.
- Keep JavaScript minimal and inline/local unless there is a clear reason to separate or add tooling.
- Prefer local image assets already in `assets/img/`.
- Preserve the existing static deploy model.

## Important Content And SEO Details
- Main entity: `Dra. Mayra Valois`.
- Business type in structured data: `Dentist`.
- Location: Cali, Colombia.
- Contact data appears in schema and should stay consistent across pages:
  - Phone: `+57 319 433 4443`
  - Email: `contacto@mayravalois.com`
  - Address: `Calle 2a Oeste #73d -06`, Cali, Colombia
- Social profiles currently referenced:
  - Instagram: `https://www.instagram.com/dra.mayravalois`
  - Facebook: `https://www.facebook.com/people/Dra-Mayra-Valois/100049261369978/`
- When changing services, update all relevant places: navigation/links, service pages, structured data, `sitemap.xml`, and any visible service lists.

## Service Pages
Existing service directories include:
- `cirugia-oral`
- `endodoncia`
- `implantes-dentales`
- `odontologia-estetica`
- `odontologia-preventiva`
- `ortodoncia`
- `periodoncia`
- `rehabilitacion-oral`

## Working Rules For Codex
- Run `git status --short` before editing.
- Read the relevant HTML/CSS before changing layout, SEO, or content.
- Keep edits scoped to the requested change.
- Do not rewrite unrelated sections or reformat entire files.
- Do not revert user changes unless the user explicitly asks.
- Preserve existing metadata style: canonical tags, Open Graph, Twitter cards, and JSON-LD structured data.
- For visual changes, check both desktop and mobile behavior.
- For SEO changes, verify title, description, canonical URL, social tags, structured data, `robots.txt`, and `sitemap.xml` when relevant.

## Quality Checks
- Use `rg` for search.
- Inspect changed files with `git diff` before finishing.
- If modifying UI, verify text does not overlap or overflow on small screens.
- If adding images, keep paths local, use descriptive filenames, and consider weight/performance.
- If committing, review for accidental secrets or private data before staging.

## Session Startup Prompt
When starting a future session, ask Codex to:

```text
Lee AGENTS.md, revisa git status y mira los archivos relevantes antes de editar.
```
