# Changelog

All notable changes to the Bao To Me website are recorded here.

Format: `## [version] — YYYY-MM-DD` followed by bullet points grouped by type.

---

## [1.5.2] — 2026-05-05

### Spacing
- Replaced fixed `7rem`/`8rem` section padding with responsive `clamp(3rem, 7vw, 5rem)` so spacing smoothly scales between breakpoints
- Desktop section padding: 112–128px → 72–80px (industry-standard for marketing sites)
- Mobile section padding: 64–80px → 40–56px
- Removed v1.5.1 mobile-only padding override (clamp now handles all viewports)

---

## [1.5.1] — 2026-05-05

### Mobile UX
- Menu tabs: 34px → 45px tall (above Apple's 44px tap-target minimum)
- Menu cards: 441px → 383px tall (≈2 fit per screen instead of 1.9), photo aspect 4:3 → 16:10 on mobile
- Contact section: BOOK A TABLE + WHATSAPP US no longer wrap awkwardly; now stack as 3 full-width buttons (Book / WhatsApp / Call) — added a tappable Call CTA with the phone number
- Address now opens Google Maps when tapped
- Bumped tap area on small links (review "Verified on Google", press "Read the story", footer Instagram, "Open in Google Maps") to ≥42px via padding
- Floor for tiny mobile text raised from ~9.9px to ~12.5px
- Section vertical padding 96–128px → 64–80px on mobile (less wasted whitespace)

---

## [1.5.0] — 2026-05-05

### Added
- Full menu photography: every menu item now has a real photo (cream/cloud-motif style for visual consistency); `context/menu/CATALOGUE/` populated with 40 dish photos
- New "Weekend Specials" tab with 3 dishes: Hainanese Chicken Rice, Tofu Dan Dan Mian, Chicken Dan Dan Mian
- Our Space section: redesigned with asymmetric staggered photo grid (4 photos), fade-in-from-blur reveal animation on scroll, and "Reserve a Table" CTA on the section
- 2 new interior photos for Our Space gallery (`BAOTOME_DAY1_6624-4-2.jpg`, `BAOTOME_DAY2_7418-Edit.jpg`)
- Proper favicon set: `favicon.png` (192px), `favicon-32.png`, and `apple-touch-icon.png` (180px) for iOS
- Dedicated OG image at `og-image.jpg` (1200×630, 131KB) for clean social link previews

### Changed
- Removed all menu prices (priceless menu)
- Removed Beverages tab and 7 drinks (Lemon Ice Tea + 6 kombuchas/teas) from menu
- Removed Dessert Bao Basket
- Removed red category section headers (e.g. "Baos (3 pcs)") to reduce visual clutter — category is already clear from the active tab
- Marquee strip: "Kombucha" → "Dan Dan Mian" (since drinks were removed)

### Fixed
- Empty bordered cells in tabs with fewer items than columns (CSS grid `auto-fill` → `auto-fit`)
- Menu category section headers no longer render

### Performance
- Resized 4 Our Space photos from 29.2 MB total → 643 KB (98% reduction). Photos were 5–11 MB each; now max 1400px wide at JPEG q82
- Replaced 2.6 MB OG image (`_T3A9645.jpg`) with optimized 131 KB `og-image.jpg`
- Replaced 71 KB favicon (with spaces in filename) with 8.3 KB optimized variants at clean root paths

### Removed
- 6 separate menu panels collapsed into category-headed panels with banner artwork (kept 6 panels but removed banners)
- Lightbox click-to-zoom on Our Space gallery (cleaner, no longer needed)

---

## [1.4.0] — 2026-03-23

### Added
- Press section: replaced 3 placeholder cards + 3 "more coverage coming soon" slots with 6 real press mentions (The Hindu, Economic Times, TheStyle.World, BW Hotelier, Restaurant India, HospiBuz)
- All press cards now link to real published articles (external links with `target="_blank"` and `rel="noopener noreferrer"`)
- `context/press/README.txt` — new press context directory for staging press assets

### Fixed
- Google Maps embed URL updated to use business name search instead of raw coordinates for better reliability

---

## [1.1.0] — 2026-03-19

### Fixed
- Accessibility: added `aria-hidden="true"` to all decorative marquee strips
- Accessibility: added `lang="zh"` to all Chinese text (`包给我`)
- Accessibility: added `role="img"` and `aria-label` to all dietary flag dots (veg, non-veg, pork, egg, spicy)
- Accessibility: added focus trap to reservation modal (keyboard navigation stays inside modal)
- Accessibility: added `tabindex="-1"` to hero section so skip-to-content link works
- SEO: added canonical URL, Open Graph tags, Twitter Card tags, favicon, and theme-color
- SEO: enriched schema.org structured data with `aggregateRating`, `image`, `hasMap`, and `menu`
- Performance: trimmed Google Fonts to only weights actually used (removed 300, 500, italic variants)
- Performance: added explicit `width` and `height` to space/interior photos to prevent layout shift (CLS)
- Content: moved Tori Katsu Sando and Prawn Toast Mantou to the correct "Appetizers" tab
- Content: corrected spelling of "Shichimi" (was "Sichimi") throughout
- Content: replaced "Ramen" with "Udon" in marquee (Ramen is not on the menu)
- Infrastructure: fixed `.gitignore` pattern for filename containing brackets

---

## [1.0.0] — 2026-03-18

### Added
- Initial website: single-page HTML/CSS/JS for Bao To Me restaurant
- Sections: hero, about, menu (tabbed), space gallery, reservations, footer
- Schema.org Restaurant structured data
- Reservation modal with Dineout embed
- Responsive layout, custom typography (Laila + Nunito)
