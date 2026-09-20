# CHANGELOG — Aniruddh Parmar Portfolio

## v1.3.0 — 2026-09-20 · "The Shipment" redesign
### Domain
- Default domain changed: `aniruddhprmr.com` → `aniruddhparmar.arceedeximhouse.com`
- Cloudflare: CNAME `aniruddhparmar` → `aniruddhprmr.github.io`, proxied
- GitHub Pages: custom domain set to `aniruddhparmar.arceedeximhouse.com`, HTTPS provisioned
- All SEO (canonical, OG, Twitter, JSON-LD, robots.txt, sitemap.xml) updated to new domain
### Concept
Scrolling the page follows a shipment: **Origin (Kutch) → Manifest → Port → Customs → Delivered.**
A journey rail on the right (desktop) tracks the "cargo" as you scroll; routes draw themselves on the About and Contact sections.

### New
- Cinematic hero: sticky 440vh scene, scroll-scrubbed video (lerp + WebCodecs frame bank, video-seek fallback), 3 sequential text phases
- Line-mask headline reveals, clip-path portrait reveal, fade-up reveals
- Marquee strip, paper-grain texture, scroll progress bar
- Track-record "ledger" with count-up and ON RECORD stamp
- Expertise: pinned horizontal scroll on desktop (stacked cards on tablet/mobile)
- Projects as tilting "document" cards
- Contact as dark "Delivered" finale with route line + stamp
- Desktop-only cursor ring, tilt and magnetic buttons
- Optional inquiry form / email / WhatsApp (auto-appear when configured in CONFIG)

### Fixed
- `mailto:#` dead link removed (email/WhatsApp are now config-driven)
- Hero image filename mismatch removed (no longer needed)
- Generated missing `og-image.jpg`, `logo.png`, `favicon.svg`
- Duplicate `</body></html>` removed
- GitHub / LinkedIn icons replaced with correct paths
- JSON-LD: removed non-functional SearchAction, full-URL `@id`s
- `theme-color` now static in `<head>`
- Title shortened to ~65 characters

### Performance
- Portraits: 1.5 MB → ~150 KB (WebP, cropped to 4:5, blurred side-bars removed)
- Fonts: 3 families / ~15 weights → 2 families / 9 weights
- Video work only starts after page load; frame bank skipped on phones, low-memory devices, Save-Data and reduced-motion

### Accessibility
- Text-safe bronze (#8a6a2e, 4.7:1) replaces decorative gold for text; muted text darkened
- Carousel: pause button, swipe, arrow keys, no autoplay under reduced motion, pauses off-screen/on hover
- Mobile menu: Esc closes, scroll lock, inert when closed
- Content stays visible with JavaScript off
- `prefers-reduced-motion`: no smoothing, no pinned scroll, no autoplay, marquee stopped

### To do by owner
- Set `CONFIG.CONTACT_EMAIL` and `CONFIG.WHATSAPP` (top of the script)
- Replace `CONFIG.VIDEO_SRC` with footage you own/licensed (ports, containers, textiles)
- Confirm the `@AniruddhParmar` Twitter/X handle exists
