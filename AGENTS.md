# AGENTS.md

## Architecture
- Static site, with no framework and no build step. Netlify publishes `public/` (see `netlify.toml`).
- `public/index.html` holds everything: the markup, the inline `<style>` and an inline IIFE `<script>`. The script contains a hash/data-go router across `section.page` elements, the booking form validation, the slot-grid picker, client-file generation, printing, and `.ics` and mailto reminders.
- Persistence happens only on the client, through `localStorage` (with an in-memory fallback). No backend exists.
- `public/img/` holds self-hosted images (originally from a Z.AI CDN; filenames are the original file IDs). Some `.png` files are actually JPEG data.

## Conventions
- The content is in Italian. Keep the compact class names and the minified-ish style of the existing code.
- If server-side storage of bookings is ever needed, use Netlify Forms or Netlify Database rather than an external service.
