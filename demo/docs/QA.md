# QA — Flowers by Kodie factual-archive rebuild

**Current state:** FAIL — REDESIGN DIRECTION. User-rendered Desktop evidence identified a cropped Hero and an unbalanced 2025 story composition. F-021/F-022 remain local-only editorial originals; no deployment or customer contact has occurred.

**Actual Demo Minutes:** UNKNOWN — an accurate start timer was not preserved across the two direction resets. `SOP COST REVIEW` is therefore flagged rather than inventing a duration.

## Static checks — 2026-08-31

- Eight unique visible images resolve: six original concepts and two user-directed, unmodified Ipswich.co.uk editorial originals. Each has a unique placement and appears in `IMAGE_LEDGER.md` and `ASSET_INVENTORY.csv`.
- Only documented `mailto:[REDACTED_EMAIL]` actions are interactive. The historic telephone is readable but not a `tel:` link.
- The visible marker is the permitted low-interference text: `Independent concept preview`.
- Every time-sensitive address, hours, collection, contact route, seasonal plan and opening-year record is visibly framed as a dated/archive record. `FACT_ARCHIVE_MAP.md` maps each fact to its source and forbidden current meaning.
- No form, payment, booking, login, map, social link, price, review, certification, invented project or current delivery/stock claim exists.
- Native links have visible `:focus-visible` treatment; reduced motion disables transition and smooth scrolling.

## Real-browser evidence — 2026-08-31

- Local Playwright browser session at **390×844**: `innerWidth=390`, `documentWidth=390`; no horizontal overflow. First Tab focused the hero email CTA; console reported **0 errors / 0 warnings** after the inline favicon fix.
- Local Playwright browser session at **1440×900**: `innerWidth=1440`, `documentWidth=1440`, full document height 7490px.
- Desktop top/middle/bottom editorial integration: `screenshots/desktop-top-editorial-final-playwright.png`, `screenshots/desktop-middle-editorial-final-playwright.png`, `screenshots/desktop-bottom-editorial-final-playwright.png`.
- Mobile top/middle/bottom editorial integration: `screenshots/mobile-top-editorial-final-playwright.png`, `screenshots/mobile-middle-editorial-final-playwright.png`, `screenshots/mobile-bottom-editorial-final-playwright.png`. Each is an exact 390×844 viewport.
- The earlier Chrome headless images remain historical capture artifacts only; Playwright is the current viewport evidence because it enforces the requested CSS viewport.

## Gates

- CLIENT-VISIBLE INTERNAL-TEXT GATE: PASS — no implementation/process/rights language is customer-visible; the permitted concept marker is present.
- BOTTOM 40% COMMERCIAL QA: PASS for a local concept: dated archive context leads to a single honest email route; no historical plan is presented as a service.
- INDEPENDENT VISUAL ACCEPTANCE: FAIL — superseded by user-rendered visual-direction feedback; re-review required after the layout rebuild.
- CLIENT-SHOWABLE DEMO: FAIL — visual direction is not accepted, and F-021/F-022 are user-directed local-only third-party editorial originals whose publisher/photo rights and customer authorisation are NOT VERIFIED.
