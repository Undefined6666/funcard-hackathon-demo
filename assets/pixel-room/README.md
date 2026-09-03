# Pixel room asset contract

This folder is the handoff point for Aseprite exports. The Phaser scene currently
draws a complete fallback room so the MVP is playable before final art arrives.

Recommended exports:

- `room-background.png`: 960 × 560, opaque, background only.
- `room-foreground.png`: 960 × 560, transparent occlusion layer.
- `traveler-walk.png`: four 80 × 128 side-view frames in one horizontal strip.
- `traveler-front.png`: one 80 × 128 front-view frame for creator and card views.

Export with nearest-neighbor scaling, no smoothing, and transparent canvas for
character/foreground files. Keep the walkable floor inside y=350…520 and the
portal entrance around x=804…928 so artwork can be replaced without changing
movement code.
