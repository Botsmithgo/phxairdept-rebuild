# Phoenix Air Department — 2026 Rebuild (Pitch Site)

## Purpose

A completely fresh, high-conversion redesign of phxairdept.com (Phoenix Air
Department — Tempe, AZ HVAC + plumbing). Built as a **sales/pitch artifact** for
the local-services agency: hand them a dramatically better site than the dated
WordPress/Genesis template they run today. Single long-scroll landing page,
built for the Phoenix HVAC buyer (emergency no-cool panic + planned $8–15k
replacement anxiety).

This is **not** a copy of their current site and **not** a templated research
clone. It keeps their brand colors and expresses them through an original
**"Editorial Bright"** art direction.

## Source Files

- Deploy entry / canonical: `index.html` (single-file, vanilla HTML/CSS/JS)
- Assets: `assets/scraped/` (their real images), `assets/curated/` (stock fills),
  `assets/generated/` (AI hero + key visuals)
- Recon + research: `.research/teardown.md`

## Production

- Public URL: TBD — deploy to Vercel only after Youssef approves the local build
- Planned Vercel project / GitHub repo: `phxairdept-rebuild` (under `Botsmithgo`)
- **Auto-deploy (once connected):** push to `main` → Vercel builds + deploys.
  No build step (static HTML, `outputDirectory: "."`).

## Deploy workflow (after approval)

1. `git init` → commit → create private GitHub repo `Botsmithgo/phxairdept-rebuild`
2. Connect repo to Vercel (auto-deploy on push to `main`)
3. Edit `index.html`, commit, push → live in ~10s

## Design system — "Editorial Bright"

- **Direction:** bright white, magazine/editorial. Oversized confident display
  type, asymmetric layouts, generous whitespace, big crisp full-bleed imagery,
  hairline rules + numbered section markers. Apple-meets-trade.
- **Brand palette (their real colors — keep):**
  - Signature red: `#E21319` (the one electric accent — CTAs, links, underlines)
  - Ink: `#111111` · Canvas: `#FFFFFF` · warm grays for structure
  - Micro-accents `#F7E700` / `#00A0D2` only if truly needed
- **Type:** tight grotesk display (Inter Tight / Space Grotesk) + clean body sans
  + mono for eyebrows/labels/data.
- **Motion (all behind `prefers-reduced-motion`):** scroll-reveal, kinetic
  headlines + red underline draw-on, number counters, marquee trust strip,
  subtle image parallax/zoom, magnetic hover. No auto-rotating carousels.

## Editing rules

- Keep the **verified facts** accurate (phone, address, ROC #329176, services,
  plans, service areas) — see `.research/teardown.md`. Copy may be rewritten.
- Do **not** fabricate aggregate review counts/stars (their Google Business
  Profile is gone). Use real review **quotes + badges** only.
- "Service area" cities are real; the agency does not own trucks.
- Mobile-first; the page must never overflow the viewport. Dense rows scroll
  horizontally inside their container, not the page.
- Re-run JS syntax, HTML validation, mobile-width, interaction, and
  console-error checks after meaningful edits.

## Verified facts (quick reference)

- Phone (602) 586-6001 · info@phxairdept.com · 2130 E 5th St, Tempe AZ 85281
- Hours M–F 8–6, Sat 9–4, Sun closed · 24/7 emergency
- AZ ROC #329176 · BBB A+ · Bryant dealer · since 2015 · military/first-responder 10%
- Services: AC repair/install · heating/furnace · HVAC maintenance · new
  construction (+IAQ) · plumbing · 24/7 emergency
- Plans: Silver/Gold/Platinum ($9.99–$50/mo) · Financing: Wisetack
