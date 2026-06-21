# World Manifest — beat → asset mapping

Maps each scroll-spine beat (brief §3) to its world-skin asset (ImagineArt) and the live layer composited on top. Operator supplies ImagineArt output; the site reads paths from here. `status`: ✅ ready · 🟡 generating · ⬜ needed.

| Beat | Plate / loop (world skin) | Path | Live layer (WebGL) | Status |
|---|---|---|---|---|
| **OPEN — Tap to be known** | Café/block hero plate | `world/plates/C-cafe-block-open-01.png` | tap → ripple, amber thread → cyan emitter, grant/revoke (VeilCanvas) | ✅ plate + live layer |
| OPEN motion | `loop-tap` (plate → veo-3.1) | `world/loops/loop-tap.webm` | live glow composite | ⬜ |
| **PLACE — Your block** | Street + storefront plates; Places gallery | `world/plates/C-street-golden-*`, `world/gallery/*` | ambient pulse on scroll | ⬜ |
| **SECRET — the line** | Minimal plate / type-on-dark | `world/plates/G-secret-01.*` (optional) | — | ⬜ |
| **CARRIED — you, carried** | Theo across 2–3 places | `world/plates/D-theo-*` | amber filament tracks scroll | ⬜ |
| **REACTS — world reacts** | Café interior + counter composite | `world/plates/B-counter-composite-01.*` | green grant; blind-react light | ⬜ |
| **TERMS — on your terms** | Same place, Veil-off baseline | `world/plates/B-counter-composite-01.*` | Veil post-process ON; revoke → red dissolve | ⬜ |
| **DEVICE — the Portal** | Product stills (locked renders) | `renders/portal-hero.png` etc. | interactive glTF Portal, emissive seam | ✅ stills / ⬜ glTF |
| **SUBSTRATE — plugs in** | Car cabin, home plates | `world/plates/B-car-*`, `B-home-*` | small live handshake demo | ⬜ |
| **FINALE — city alive** | Aerial/district plate (Pack C) | `world/plates/C-aerial-district-01.*` | live cyan pulse mesh overlay (shader) | ⬜ |
| FINALE motion | `loop-city-pullback` | `world/loops/loop-city-pullback.webm` | mesh overlay | ⬜ |
| **LIVE — this is how you live** | OG-quality hero still | `renders/` or `world/plates/` | early-access form (consent-first) | ⬜ |

## Anchors (lock in ImagineArt web app before bulk generation)
1. **Style** — custom style model or standing style reference (the style recipe in `cityos-reference-image-plan-20260620.md`).
2. **Device** — custom model trained on the 9 Portal renders + Portal in Elements.
3. **Theo** — Imagine You from `theo-character-ref.png` + Elements.

## Notes
- Plates: WebP/AVIF, full-bleed; loops: WebM (poster-first), 16:9, scrubbed to scroll.
- Generated-here assets (MCP) recorded in `ASSETS.md` with model + prompt; web-app assets recorded on export.
- The 4-color glow grammar appears only on the **live layer**, never baked into plates (except Pack E calibration refs in `public/refs/`).
