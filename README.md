# LINDAI

AI-Powered Community Resilience, Security & Economic Intelligence for Laikipia and Samburu, Kenya.

**Live site:** https://atindahhillary.github.io/LINDA-AI/
**Founder:** Hillary Atindah George — atindahhillary@gmail.com

## What this is

LINDAI turns scattered incident reports (banditry, livestock theft, human-wildlife conflict, illegal grazing, drought shocks, road insecurity) into a live, GIS-mapped picture of risk for the institutions that already own this problem — county governments, Kenya Wildlife Service, National Police Service, conservancies, and NGOs.

This repository holds the public-facing pitch and impact website: the front door for investors (raising through Askya's AI Growth Platform), grant and philanthropic funders, and prospective pilot partners. It is deliberately honest about stage — pre-revenue, concept stage, self-funded to date — because that transparency is a credibility asset with funders, not a weakness to hide.

## Tech stack (MVP)

Static, dependency-free front end — fast to load on the low-bandwidth connections this project's own users have, and simple enough to deploy from any static host:

- Semantic HTML5 (`index.html`)
- Vanilla CSS with design tokens (`assets/css/style.css`) — no framework, no build step
- Vanilla JS for nav, scroll-reveal, and active-link tracking (`assets/js/main.js`)
- Google Fonts (Inter / Space Grotesk), self-contained SVG icons and favicon

```
LINDA-AI/
├── index.html
├── assets/
│   ├── css/style.css     # design tokens + all styling
│   ├── js/main.js        # nav, scroll-reveal, active nav state
│   └── img/favicon.svg
└── README.md
```

## Running locally

No build step required. Either open `index.html` directly in a browser, or serve it locally:

```bash
python -m http.server 8080
# then open http://localhost:8080
```

## Roadmap: MVP → Scale

This site is intentionally the smallest thing that ships credibly. As LINDAI itself moves from pitch to pilot to product, the front end is expected to grow in stages:

1. **MVP (this repo today)** — static pitch/impact site on GitHub Pages. Zero infrastructure cost, fast to iterate, easy for any funder or partner to review.
2. **Content scale** — pull copy/metrics into structured data (JSON/CMS) so traction numbers, pilot status, and partner logos update without touching markup.
3. **Partner portal** — a authenticated, role-based entry point (ranger / county desk / KWS / conservancy) linking out to the actual LINDAI GIS dashboard product described on this site.
4. **Product front end** — the marketing site and the LINDAI operational dashboard (incident capture → AI analysis → GIS mapping → role-based response) converge behind a shared design system, likely on a framework (e.g. Next.js) once the product itself is in active pilot use.

## Content source

Copy and figures are drawn directly from the founder's pitch deck (`LINDAI_Askya_Pitch_Deck.pptx`). Traction figures (funding raised, customer count, pilot status) should be updated here the moment they change on the ground — this site should never claim more than the pitch deck and the founder are prepared to stand behind.
