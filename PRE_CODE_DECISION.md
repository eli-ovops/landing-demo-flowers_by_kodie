# Flowers by Kodie — Pre-code Decision

**Scope:** local L0, static, client-showable concept only. No publishing, contact, account action, data collection, ordering, payment, booking, or customer-system change.

## Authority read receipt

- `AGENTS.md`: full read on 2026-08-31 before this document and before any customer-visible code.
- `PROJECT_CORE.md`: full read on 2026-08-31 before this document and before any customer-visible code; applicable rules include Demo Production v1.1, First-pass Gate, 14.3A/B, 14.4/14.4A and 14.6.
- `website-delivery-sop/SKILL.md` and DS-002B V2.5: full first-website-task read on 2026-08-31; SHA/mtime in Skills receipt below.

## Facts and asset coverage

- Flowers by Kodie is an independent florist at 6 High Street, Debenham. Kodie Brooke runs it. The public record supports bespoke bouquets/arrangements, tribute flowers, a florist plus garden/gift-shop direction, collection from Ipswich, and the existing business email.
- The page will make no claim about delivery, price, availability, stock, reviews, awards, team, completed events, or checkout.
- Asset: one original concept still-life, generated for this local concept only. It is not a photo of the shop, Kodie, customer work, or a real tribute. Its role is mood and floral craft, not proof.

| Fact / asset class | State | Evidence / treatment | Page role or non-use reason |
| --- | --- | --- | --- |
| Name / local identity | USE | Ipswich local-news article, 15 Oct 2025; FindGlocal P311-A snapshot 30 Aug 2026 | Hero and footer identify Flowers by Kodie, Debenham only. |
| Kodie Brooke | USE internally only | Ipswich article identifies the owner | Not named in visible copy: first-name familiarity is unnecessary and avoids overstating current owner contact. |
| Bouquets / arrangements | USE | P311-A descriptor | Hero and bouquet route. |
| Tribute flowers | USE | P311-A post, 29 Jul 2026 | Tribute route, without price, availability or catalogue claims. |
| Garden / gift-shop direction | USE | P311-A posts, 25 Jun and 8 Jul 2026 | Shop note, phrased as a shop detail rather than a promise. |
| 6 High Street / hours | USE | P311-A address/hours section | Footer shop note only; no map or navigation claim. |
| Email | USE | P311-A, same order post | Mailto CTA only. |
| Logo / verified brand type / brand colours | UNAVAILABLE | No current owned brand asset or verified guidelines | Wordmark is plain text, no imitation logo. Palette originates with concept art, not claimed as brand colour. |
| Customer photos / social images | DO NOT USE | No customer permission or licence proof | Never downloaded or represented as owned. |
| Reviews, prices, delivery, catalogue, staff, awards, availability | DO NOT USE | No verified basis fit for this concept | No display or implication. |
| Booking, checkout, inventory, payment | DO NOT USE | Outside £600 static scope | No UI, link, placeholder or pseudo-control. |

## £600 Purchase Thesis

For a Debenham florist whose bouquets, tributes, shop identity and enquiry route currently live in a chronological third-party feed, a focused owned page can let a visitor immediately choose the right occasion, understand the local shop, and make an email enquiry—without inventing ecommerce or maintenance-heavy features.

## UK visual reference set (checked 2026-08-31)

1. https://suffolkflorist.co.uk/ — retain the calm regional specificity and services-to-enquiry clarity; do not copy layout, photos, words or identity.
2. https://www.occasionsflorist.co.uk/ — retain occasion-led structure and compassionate tone for funerals; do not copy claims or imagery.
3. https://www.perrystreetflowers.co.uk/ — retain fast service-category recognition; do not copy card styling or content.
4. https://lilysflorist.co.uk/ — retain the small-independent warmth and compact service hierarchy; do not copy its visual system.

All four were directly opened, without login, on 2026-08-31: Suffolk Florist (weddings/workshops/contact visible), Occasions (occasion navigation and funeral reassurance visible), Perry Street (gift/wedding/funeral hierarchy visible), and Lily’s (occasion navigation and local contact close visible). Application mapping: Suffolk Florist informs the quiet regional **shop note**; Occasions informs the compassionate **tribute route**; Perry Street informs the fast **occasion choice**; Lily's informs the compact **email close**. None supplies visual assets, copy, code, brand claims or layout reproduction.

## Design Read and dials

**Reading this as:** a rural Suffolk independent-florist concept for local gift buyers and families planning a tribute, with a quiet editorial garden language leaning toward an asymmetric print-inspired shopfront.

- `DESIGN_VARIANCE: 7` — asymmetric rail, oversized botanical crop, and staggered service rhythm.
- `MOTION_INTENSITY: 3` — tactile hover/focus feedback only; no automatic animation.
- `VISUAL_DENSITY: 4` — generous hierarchy but enough practical route information to act.

## Two materially different directions

### A — Garden ledger (selected)

Ink-blue page with green botanical imagery; a left-side shop ledger introduces Debenham, while oversized occasion words step down the right. The bottom becomes a compact local shop note and email hand-off. It makes the directory-to-owned-page contrast visible without fake portfolio content.

**Bottom 40%:** a non-gallery, proof-led “from the flower room” note makes the real High Street / garden-and-gift-shop detail visible, then an understated email invitation provides the same route the current record publishes. **Purchase thesis difference:** selection turns practical village-shop context into reassurance, rather than just an attractive bouquet page.

### B — Flower-room invitation (not selected)

Light paper gallery with a central bouquet image, three vertical occasion panels, and a workshop-style contact close. It is calmer but too close to a generic premium florist and makes the small High Street identity less immediate.

**Bottom 40%:** a picture-led seasonal note and a simpler contact close. **Purchase thesis difference:** it would sell atmosphere first; it is rejected because it cannot prove the Debenham shop identity as quickly as A.

**Selection rationale:** A carries a distinctive “village flower-room / sign-painter ledger” visual language, gives a five-second service choice, and lets the verified shop address and email act as real commercial information rather than filler.

## Implementation map

| Page responsibility | Verified basis | Implementation |
| --- | --- | --- |
| Hero identity | Flowers by Kodie, Debenham, bouquets/arrangements | `demo/index.html` `.hero` |
| Occasion paths | bouquets, tribute flowers, gift-shop direction | `.occasions` cards |
| Trust/reassurance | named High Street shop; one-year High Street/garden shop update | `.shop-note` |
| Conversion | published business email | `mailto:[REDACTED_EMAIL]` CTA |
| Visual distinction | original concept image only, not factual proof | `assets/kodie-concept-floral-still-life.png` |
| Bottom 40% / close | High Street identity, gift/garden-shop direction, email | `.shop-note`, `.contact-close`, footer |

**Cross-demo similarity check:** compared against `/Volumes/EXTERNAL/海外落地页/client_uk_jl_and_tm_cleaning/demo_2026-08-24/` and `/Volumes/EXTERNAL/海外落地页/client_uk_tranquil_touch_relaxation_therapy/demo_v2_20260823/`. The selected direction intentionally differs on: `(1)` asymmetrical side-ledger hero rather than generic full-width/central treatment, `(2)` ink-blue/green rather than either project's palette, `(3)` no real-customer asset reuse, `(4)` occasion paths rather than service-card grid, `(5)` High-Street note rather than gallery/process, `(6)` mailto-only CTA rather than booking/form path, `(7)` proof-led Bottom 40% rather than reviews/gallery, `(8)` no decorative pseudo-logo, `(9)` no ambient/continuous motion, `(10)` mobile keeps the ledger strip as a compact factual header rather than collapsing into the same card stack. Similarity hits: `0/10`.

**Anti-template guards:** no centred hero, no feature-card trio, no fake review/gallery, no cookie/banner UI, no generic “ready to transform” closing, no secondary colour family, and no repeated eyebrow labels.

## Skills execution receipt

- **website-delivery-sop — USED:** classified L0 only; DS-002B V2.5 read, SHA-256 `5b70133e7a155a713c130d07d883afffbd1f57eaa7bfc7c2e2c3dfc9f9bb926a`, mtime `2026-08-09T16:00:52+0800`. It fixes the no-deploy/no-data/no-production boundary and requires P0–P3 records in this decision, fidelity map, image ledger and QA.
- **design-taste-frontend — USED:** the Design Read, dials, two genuinely different directions, asymmetric hero and one-theme palette directly map to selectors above; it rejects a centred template hero, generic feature-card rhythm and beige/brass craft default.
- **media-use — USED within authorised limits:** its asset provenance and “frozen local file + ledger” model is applied. Provider setup/login/install was not run because it is not authorised. The original local concept image is assigned to one placement and recorded in `demo/docs/IMAGE_LEDGER.md`.

## Pre-code reviewer hand-off

Reviewer must verify fact coverage, asset honesty, direction distinction, £600 thesis, anti-template safeguards, scope and mobile mapping before any customer-visible HTML/CSS/JS is written.

**PRE-CODE GATE: PASS — independent read-only review, 2026-08-31.** Scope is limited to authorised local static Demo coding.

---

# V2 Full-page Visual Storyboard — REDESIGN DIRECTION

**Status:** `FAIL — REDESIGN DIRECTION`. The previous one-image Hero-led composition is retired. This V2 plan replaces its visual architecture before customer-visible code is changed.

## Current UK reference refresh — 2026-08-31

1. `https://suffolkflorist.co.uk/` — full page alternates service explanation, work imagery and a contact close. Apply: visual route cards, not copied imagery or copy.
2. `https://www.occasionsflorist.co.uk/` — uses a distinct visual and gentler text treatment for funeral work. Apply: quiet tribute beat, no claim about customer work.
3. `https://www.perrystreetflowers.co.uk/` — establishes service categories with photography before its contact path. Apply: three occasion-specific visual panels, not ecommerce controls.
4. `https://lilysflorist.co.uk/` — uses separate bouquet, wedding and funeral images with a practical local contact close. Apply: distinct subject/crop per page beat, without copying assets, reviews or claims.

## Visual distribution rule

There are six separate original concept assets. No asset, crop or variation is reused. Every primary commercial beat has a different layout family and a visual role; no two major consecutive sections are text-only.

| Beat / selector | Visual task and layout family | Fact mapping | Asset / rights | Mobile crop | Motion purpose |
| --- | --- | --- | --- | --- | --- |
| Hero | Wide flower-worktable still life; split ledger overlay | bespoke bouquets/arrangements, Debenham | original concept visual 01; no customer claim | retain flowers at right edge | none; static hierarchy |
| Bouquet route | Tall, close bouquet portrait beside concise route | bouquets/arrangements | original concept visual 02 | centred bouquet | CTA hover feedback only |
| Tribute route | Horizontal blue-and-white tribute still life with muted copy panel | public blue tribute post only | original concept visual 03 | centre the arrangement | CTA hover feedback only |
| Flower room | Architectural/detail image of a non-identifying florist workroom and gift/garden textures | garden/gift-shop direction, no real shop portrayal | original concept visual 04 | retain worktable / plants | none |
| Handcraft / proof | Hands wrapping stems; process-led editorial layout | bespoke handmade arrangement concept, never a real Kodie project | original concept visual 05 | retain hands and paper wrap | none |
| Closing | Dusk-like single-vase floral mood, intimate full-bleed close | email enquiry only | original concept visual 06 | centre vase | button hover feedback only |

**Visual/asset safety:** every visual is generated from a distinct prompt and is an original concept image; it must not be described as the shop, Kodie, a customer order, a real tribute, a testimonial or proof of a delivery. Existing customer/news/social images and logo remain excluded.

**CLIENT-VISIBLE INTERNAL-TEXT GATE:** V2 removes `Independent concept preview` and every other internal/range/design-process label from the customer-visible page. Governance language remains only in these local docs.

**V2 PRE-CODE GATE: AWAITING INDEPENDENT REVIEW**

---

# V1.2 authority reset — asset-investigation phase

**Status: `FAIL — REDESIGN DIRECTION`.** On 2026-08-31, Demo Production v1.2 superseded every preceding visual direction, image plan and pre-code outcome in this file. The existing `demo/index.html` is frozen as an invalid historical draft; it is not a coding base and cannot be shown to a customer. No new customer-visible HTML/CSS/JS may be changed until the v1.2 asset investigation, storyboard and independent review are complete.

The authoritative investigation and per-asset decisions are in `demo/docs/CUSTOMER_PUBLIC_INTELLIGENCE.md` and `demo/docs/ASSET_INVENTORY.csv`. In particular, public editorial images, directory/social hints and the pre-v1.2 generated image are not silently carried forward.

**V1.2 PRE-CODE GATE: NOT YET REQUESTED.**

## V1.2 proposed purchase thesis and visual storyboard

**£600 Purchase Thesis:** the visible public record is scattered between a local-news story and a third-party directory, while a buyer has to infer whether this is a local florist for a gift, a wedding or a tribute. A concise owned landing page can turn the verified Debenham florist identity and occasion breadth into a clear, respectful enquiry journey. It will not pretend to be a shop catalogue, delivery service or a portfolio of completed work.

### Current UK visual references (rechecked 2026-08-31)

1. [The Suffolk Florist](https://suffolkflorist.co.uk/) — a local independent makes service scope and direct contact easy to find while using photography between content beats. Apply: local specificity and image-led rhythm; do not copy its content, assets, testimonial or form.
2. [Occasions Florist](https://www.occasionsflorist.co.uk/) — separates weddings and funeral flowers, with distinct imagery and gentler funeral wording. Apply: a discrete, compassionate tribute beat; no borrowed imagery or claims.
3. [Lily’s Florist](https://lilysflorist.co.uk/) — makes bouquet, wedding and funeral paths visually distinct and closes with contact/context. Apply: varied visual functions and occasion recognition; no product data, reviews, prices or gallery structure.

**Design Read:** a small, young Debenham flower room presented as a quiet series of tactile floral moments: ink, pressed paper, restrained blue and living green—not a generic luxury florist ecommerce site.

- `DESIGN_VARIANCE: 8` — a sequence of different editorial compositions, not repeated cards.
- `MOTION_INTENSITY: 3` — focus/hover-only feedback; no automatic motion and no motion-design skill trigger.
- `VISUAL_DENSITY: 5` — prominent photography with sparse, factual copy and a single email path.

| Commercial beat | Visual task / composition | Exact fact mapping | Source / rights | Mobile crop and interaction purpose |
| --- | --- | --- | --- | --- |
| Hero: place and flower craft | Wide, original still-life that holds a deep-blue paper title panel; no shop frontage, people, logo or real arrangement. | Flowers by Kodie; Debenham; florist. | New original concept image; never presented as customer work. | Image becomes a tall crop with the bouquet subject retained; CTA hover/focus confirms the enquiry route. |
| Occasion: bouquets | Vertical hand-tied bouquet image beside a short “everyday moments” route, using a loose editorial frame. | Public evidence supports bouquets/arrangements. | New original concept image. | Full-width image before route copy; no product/price button. |
| Occasion: tribute | Low, horizontal arrangement image and a calm inset text panel—not an online funeral product grid. | Public record supports funerals/tribute work; no specific live design claim. | New original concept image, conceptual not a real tribute by Kodie. | Arrangement stays central; interaction only makes email action clear. |
| Method: flower-room care | Detail of hands conditioning/wrapping stems with a text rail explaining bespoke floristry in general, without calling it a Kodie process. | Floristry training and bespoke/occasion evidence; no undocumented operating process. | New original concept image; no identifiable person. | Hands and material retain crop; scroll reveal is avoided. |
| Local proof: Debenham invitation | Original non-identifying floral worktable / entrance atmosphere, paired with a factual Debenham location note only. | Debenham identity; address withheld unless live-reverified. | New original concept image. | Worktable scene anchors the section, never a shop photo. |
| Closing: meaningful enquiry | Quiet single-vase evening still life with a single email CTA. | Published business email only if the live-contact decision remains acceptable. | New original concept image. | Vase subject remains centered; clear keyboard-focus mailto. |

This creates six different visual tasks and layout families. There are no consecutive text-only major sections, no duplicate crop, no background colour pretending to be a commercial visual, and no customer/image asset is falsely represented.

### Two material directions considered

**A — Debenham flower-room folio (selected):** a dark ink/paper editorial sequence where each occasion or customer need has its own photographic moment. The commercial mechanism is recognition first, then a calm email invitation. It can truthfully use sparse facts without fake proof.

**B — Village-market noticeboard (rejected):** bright paper signs, labelled sections and garden-shop motifs. It would foreground the gift-shop/garden direction too heavily, even though its current operation is not live-verified, and risks turning historical plans into claims.

**Selection rationale:** A gives bouquets, tribute work, making and local context visibly different roles while placing only verified facts in copy. It is farther from the prior one-image / textual-ledger direction and from standard florist shop templates.

### V1.2 skill receipt / implementation mapping

- **website-delivery-sop — USED:** the v1.2 reset is recorded before customer-visible edits; it keeps this work local L0 with no deployment, contact, data collection, login or external write. The resulting gate evidence will be in this decision file, the intelligence report, inventory, ledger, fidelity map and QA.
- **design-taste-frontend — USED:** the Design Read, three dials, two material directions, no-card-grid constraint and six distinct visual/layout tasks directly shape the later DOM and CSS rather than merely adding a theme.
- **media-use — USED within current authority:** a full source/provenance, rights and treatment pass produced `CUSTOMER_PUBLIC_INTELLIGENCE.md` and `ASSET_INVENTORY.csv`; blocked social/editorial assets are excluded rather than copied. Provider installation/login is not authorised, so none was performed. Any new image will be frozen locally, uniquely hashed and registered before use.

**CTA decision:** the final local concept may include only `mailto:[REDACTED_EMAIL]`, because the retained 2026-08-30 public directory evidence showed it alongside the business name and order contact. This is not a sending action, delivery/current-validity claim or customer authorisation. Phone, map, hours, Instagram/Facebook and every other live-contact claim are excluded. If a reviewer finds the evidence threshold inadequate, the Demo must remain without that CTA and cannot claim conversion readiness.

**Requested independent review scope:** facts/assets mapped or excluded; no current/historical fact drift; no one-image-plus-text architecture; six visual beats have distinct business functions; customer specificity is not simulated with unlicensed media.

**V1.2 PRE-CODE GATE: PASS — independent read-only review, 2026-08-31.** Reviewer conditions are incorporated in the inventory and must remain true during implementation: only F-010–F-015, one hash/one purpose per asset, no unlicensed customer material, no historical-plan claims, and no CTA beyond the documented `mailto:`.

---

# Authority refresh — official-asset reset (2026-08-31)

**Status: FAIL — REDESIGN DIRECTION.** Latest authority replaces the concept-only pre-code outcome. The current page is frozen: no official customer asset is currently attributable, and the independent reviewer also reported type-crop defects.

**Current Offer Purchase Thesis — United Kingdom / £600:** a £600 static page earns its place only if it turns official customer work and clear occasion/contact evidence into a recognisable local enquiry journey. Without an accessible, attributable official asset set, evidence cannot support a client-specific visual rebuild.

**Official-surface recheck:** no owned domain was found; Instagram candidate https://www.instagram.com/flowersbykodie/ returned a public 404 profile route; Facebook candidates redirect to login; FindGlocal is third-party and returned Cloudflare 403. No bypass/login was attempted.

**PRE-CODE GATE: BLOCKED — official customer-asset harvest unavailable.**

---

# User-directed factual archive rebuild — 2026-08-31

**User scope instruction:** incorporate the complete known factual record into the local Concept Preview in a coherent, attractive way. This is explicit user direction to use the listed factual record, while preserving source dates in internal documentation. It does not permit third-party photography, social imagery or other media reuse.

**Information architecture:** a local-shop archive rather than a generic florist catalogue:

1. **Arrival:** Flowers by Kodie, Debenham, with one clear email CTA.
2. **Occasions:** bouquets, weddings and tribute flowers.
3. **The shop:** 6 High Street, Debenham, phone, email, historic Tue–Sat hours and Ipswich collection.
4. **Kodie’s story:** 2025 opening after Level 2 floristry training; written as dated background, not a qualification badge.
5. **Seasonal local life:** first Christmas, wreaths and gifts, plus historic mentions of markets, workshops, sports-centre work, gift/garden ideas and delivery aspiration. All are visibly framed as 2025 context rather than current promises.
6. **Close:** direct email/phone, town and route selection.

**Protection rules:** no third-party image, logo, portrait or review; no invented project/gallery; no delivery, garden-centre, workshop or inventory promise; no uncited rating/award; no claim that historical details were live-verified today. Existing generated images are retained only as generic visual atmosphere, one unique asset per placement.

**Design Read:** rural Suffolk florist · cobalt archive + floral notebook · brand · SOUL 8 / SPECTACLE 3 / DENSITY 6. The rejected default is beige, brass and generic hand-lettered “artisan florist” styling. The selected direction uses a disciplined cobalt, faded rose and ink palette with date-led factual archive panels and a quiet, CSS-only tactile movement on real page actions.

**finesse-ui impact:** page will remove eyebrow overload and repeated split panels, use a locked cobalt accent, a grain substrate, six distinct layout families, reduced-motion-safe interaction and a content hierarchy that makes the added facts scannable instead of a long biography.

**PRE-CODE GATE: PASS — independent read-only review, 2026-08-31.** Every historical statement must retain its visible date/context; the telephone remains non-interactive; the existing email CTA is the only contact interaction; third-party imagery remains excluded; and `FACT_ARCHIVE_MAP.md` remains one-to-one with visible copy.

**Archive-copy contract:** FACT_ARCHIVE_MAP.md now maps every visible historical/contact fact to a source, time label and forbidden current meaning. F-004 is limited to dated archive use only. No visible text will call a historical plan a present service.

**Implementation receipt — 2026-08-31:** `finesse-ui` was used to reduce decorative label repetition, enforce a cobalt/ink editorial hierarchy, and repair the 390px type scale/min-content constraint. Its direct artifacts are the final mobile CSS and the archive/story layout families. `imagegen` was used for F-019 and F-020 only: generic training-notebook and winter-wreath concept visuals, each captioned and ledged as non-customer imagery. `finesse-brief` informed the fact-to-section grouping only; no workbench workflow was created. `frame-smith` was not used because a video/short-film deliverable is outside this authorised static-page scope.

---

# User-directed editorial-photo integration — 2026-08-31

**Authority and scope:** the user explicitly supplied two identifiable opening-story images and directed that their full original files be downloaded and integrated into this local Demo. The originals were resolved from the Ipswich.co.uk article's public Ghost image URLs and frozen, unchanged, in `demo/assets/raw-editorial/`. They remain third-party editorial material, not an official customer asset; `CUSTOMER AUTHORIZATION: NOT VERIFIED` and publisher/photo rights remain internal ledger facts. This direction does not authorise deployment, public release, customer contact, or reuse outside this local Concept Demo.

**Visual decision:** replace, rather than layer over, two generic concept beats: (1) Hero becomes the recognisable 2025 exterior/opening portrait with the Flowers by Kodie chalkboard; (2) the dated opening story becomes the real interior portrait. The generic hero (F-010) and training image (F-019) leave the visible page. This makes the first five seconds identify the owner, florist trade and location without adding unsupported business claims.

**Two considered compositions:** A — exterior portrait as Hero / interior portrait as opening-story proof (selected: strongest immediate ownership, title panel retains clear single enquiry CTA). B — interior portrait as Hero / exterior portrait as a late location card (rejected: the exterior board's business name is less effective when delayed and risks making the page read like a press clipping). Cropping is CSS `object-fit` only; no alteration, restoration, outpaint or image-to-image generation is permitted.

**Implementation mapping:** F-021 uses the existing single-image Hero container; F-022 uses the existing 2025 story visual. The service, method, archive and closing visual rhythm remain distinct, so this is an asset-fidelity revision rather than a template change. `media-use` directly produced frozen original files, hashes, source URLs and the ledger update. `finesse-ui` is retained for the hero/object-position and small-screen preflight; `design-taste-frontend` remains mapped to the selected editorial/cobalt layout direction.

**PRE-CODE GATE: PASS — independent asset-integration review, 2026-08-31.** F-021/F-022 may be used only unchanged via CSS presentation crop, remain internal-only third-party editorial assets, and must not be represented as official/customer-authorised material or current proof.

---

# User-rejected editorial-photo layout — 2026-08-31

**Status: FAIL — REDESIGN DIRECTION.** The user’s rendered Desktop evidence correctly identified a cropped Hero subject and a 2025 section with an oversized year, excessive empty field and thumbnail-sized real photograph. The prior visual PASS is superseded.

**Replacement composition:** retain F-021 and F-022 unchanged, but change their containers rather than their pixels. Hero becomes a shorter text/photo split whose photo column follows the exterior original’s landscape proportion, keeping the sign and Kodie legible. The 2025 section becomes a two-column editorial proof beat: large interior original on the left, compact dated narrative on the right; `2025` becomes a small chronological anchor inside the copy instead of a competing poster element. The service, archive and closing beats remain intact.

**Design Read / dials:** local opening story, not an editorial scrapbook · SOUL 8 / SPECTACLE 2 / DENSITY 5. The rejected direction was giant chronology + incidental photograph. The selected direction gives the real images proportion and narrative priority, with breathing room coming from controlled columns rather than empty canvas.

**Implementation constraints:** CSS layout/object-position only. Do not alter F-021/F-022, change identities, remove their signs, or make current-service claims. Re-run 1440×900 and 390×844 evidence plus the independent visual gate after the replacement layout.

**PRE-CODE GATE: AWAITING independent redesign review.**
