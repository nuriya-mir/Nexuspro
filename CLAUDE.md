# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

NexusPro is a single-page static HTML document (`nexuspro_strategy.html`) — a strategic business document for a sales ecosystem/CRM integration company. There is no build system, no package manager, and no external dependencies beyond Google Fonts CDN.

## Development

No build or install step is needed. Open `nexuspro_strategy.html` directly in a browser to preview. The project uses vanilla HTML5, CSS3, and JavaScript with no frameworks or libraries.

## Architecture

Everything lives in `nexuspro_strategy.html` (single file, ~990 lines):

- **CSS** (embedded `<style>` block): Dark theme with teal accents, CSS custom properties for theming, flexbox/grid layouts, print styles for PDF, responsive typography via `clamp()`, and CSS animations (blink, reveal effects).
- **HTML**: Hero section, 4 main content sections (Vision, Strategy, Tactics, Team), modal dialog for PDF download, footer.
- **JavaScript** (embedded `<script>` block): Drag-and-drop API for reordering tasks in the 3-month timeline, modal dialog management, PDF download via blob with fallback to browser tab.

## Key Files

- `nexuspro_strategy.html` — the entire application
- `nexuspro_strategy.pdf` — pre-generated PDF version served for download
- `logoNexusPro .png` — logo asset (note: filename has a trailing space before extension)
