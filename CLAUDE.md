# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **content staging repository** for the Bao to me restaurant website — not a code project. It serves as a structured holding area for all assets and content that will be used to build the website.

## Repository Purpose

The `context/` directory organizes all restaurant content by functional area, each with a README.txt explaining what belongs there:

| Directory | Contents |
|---|---|
| `context/about/` | Origin story, team bios, press, awards — `Bao To Me_ Company Profile.docx` is present |
| `context/brand/` | Brand guidelines — `Bao to me BrandBook.pdf` and `.ai` source are present |
| `context/logo/` | Logo files in EPS format (black, white, and colored backgrounds). Additional logos at `~/Documents/Baotome logo` |
| `context/menu/` | Menu PDFs — `MenuUpdate_22_12_25_05.pdf` is present in `context/` root |
| `context/photos/` | Food, interior, team photography. Additional photos at `~/Documents/BaoToMe-photos` |
| `context/location/` | Address, hours, parking, contact info — **not yet populated** |
| `context/reservations/` | Booking platform, links, policy — **not yet populated** |

## Website Goals

The website has two primary objectives, in priority order:

1. **Discoverability** — SEO and LLM-optimized so customers can find Bao to me through search engines and AI assistants. This means structured data (schema.org markup for restaurants), clean semantic HTML, fast page loads, and rich descriptive content about the food, location, and experience.

2. **Reservations** — Once a customer lands on the site, the primary conversion action is booking a table. The reservation flow should be prominent and frictionless.

## What to Do Here

Tasks in this repository are typically about:
- **Reading/extracting** content from the existing documents (brand book, company profile, menu PDF) to inform website copy or design decisions
- **Organizing** new assets dropped into the appropriate `context/` subdirectory
- **Building** the actual website by consuming this content (the website itself lives elsewhere — no framework or build system is in this repo)

## Key Assets

- **Brand Book**: `context/brand/Bao to me BrandBook.pdf` — primary reference for colors, typography, logo usage, and tone of voice
- **Company Profile**: `context/about/Bao To Me_ Company Profile.docx` — restaurant background, story, and copy
- **Menu**: `context/MenuUpdate_22_12_25_05.pdf` — current menu with pricing
- **Logos**: EPS vector files in `context/logo/` for three background variants
