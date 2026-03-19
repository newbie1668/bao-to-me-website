# Changelog

All notable changes to the Bao To Me website are recorded here.

Format: `## [version] — YYYY-MM-DD` followed by bullet points grouped by type.

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
