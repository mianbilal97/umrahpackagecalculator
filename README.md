# Umrah Package Calculator Pakistan

Free single-page Umrah package cost estimator for Pakistani pilgrims — all prices in PKR.

## Features

- **Pakistan-only**: 8 departure cities (Karachi, Lahore, Islamabad, Faisalabad, Sialkot, Multan, Peshawar, Quetta), PKR throughout
- Pricing engine: visa + city-wise return flights + tiered hotels (3★/4★/5★) + sharing (quad/triple/double) + season multiplier + children at 65%
- Animated results: count-up totals, per-component breakdown bars, itemized bill
- 100% client-side — no data leaves the browser
- Astro 5 static build; all illustrations in lightweight **WebP**
- SEO: semantic HTML, meta/OG/Twitter, WebApplication + FAQPage JSON-LD, ~2,000-word Pakistan-focused guide

## Price basis

Indicative estimates from published 2026 Umrah package rates in Pakistan (±10–15%). See the methodology section on the page.

## Structure

```
src/layouts/Layout.astro       # head, meta, JSON-LD, header/footer
src/components/Calculator.astro # pricing engine + UI
src/pages/index.astro          # hero + how-to-use + guide
src/styles/global.css
public/images/*.webp           # hero, how-to-use, hotel tiers, price breakdown
public/favicon.svg
```

## Run locally

```bash
npm install
npm run dev     # http://localhost:4321
npm run build   # -> dist/
```

## Deploy

Static Astro output — Vercel auto-detects the framework. No build config needed.
