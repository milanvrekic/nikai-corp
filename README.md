# nikai.ca

Static site for Nikai's printable SKS designs. Every purchase goes to the Cults3D listings.

## Pages
| URL | File |
|---|---|
| `/` | `index.html` — the three designs |
| `/sks-chassis-xcr/` | `sks-chassis-xcr/index.html` |
| `/sks-chassis-oem/` | `sks-chassis-oem/index.html` |
| `/sks-charging-handle/` | `sks-charging-handle/index.html` |
| `/xcr-modification-guide/` | `xcr-modification-guide/index.html` |
| `/parts/` | `parts/index.html` |
| `/faq/` | `faq/index.html` |

## SEO and old traffic
- `_redirects` — 301s from every old WordPress URL (shop, products, blog posts, R&D project pages, policies) straight to the matching new page.
- `sitemap.xml` and `robots.txt` — list only the four pages above.
- Structured data (JSON-LD): Organization/WebSite on the homepage, Product + BreadcrumbList on each design page, HowTo on the guide, FAQPage on the FAQ.
- `404.html` — fallback that links back to the homepage.

## Deploying
Hosted on Netlify (`netlify.toml`, no build step, publish directory is the repo root). Connect this repo to the Netlify project and every push to `main` deploys.
