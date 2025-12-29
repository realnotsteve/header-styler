# Project: Header Styler (WordPress + Elementor plugin) [browser UI theming]
Slug: header-styler

## Identity check (always do this first)
- Confirm the working directory is this plugin: header-styler
- Do not modify other plugins (crossfade-scroller, beseo) unless explicitly asked.
- Never edit files outside this plugin directory unless explicitly requested.

## What this plugin does
- Controls browser UI theming via HTML metadata, primarily:
  - <meta name="theme-color">
- May also manage related tags/behavior for mobile browsers (Safari iOS, Chrome Android).
- Includes Elementor integration for page-level or widget-level controls.

## Core priorities
- Correct meta output in the document <head>.
- Broad browser compatibility; avoid duplicated/conflicting theme-color tags.
- Progressive enhancement: if JS fails, the static theme-color should still be correct.
- Keep frontend JS light and performance-friendly.

## WordPress + Elementor conventions
- Sanitize inputs, escape outputs, capability checks, nonces for admin actions.
- Handle Elementor editor vs frontend intentionally (do not break editor UI).

## Output style (how to respond)
- Do NOT print entire files unless explicitly requested.
- When proposing changes: specify file path + hook + expected resulting HTML.

## Testing checklist
- Verify theme-color output:
  - homepage, a normal page, and an Elementor page
- Confirm no duplicate meta tags; verify no console errors.

## Attribution
- If author credit is needed in plugin code examples, use: Bill Evans