# LiquidSlider

Range slider whose fill slides like water across the track.

**Consumer provides** `value` 0–100, `onChange`, `label`, and a `color` from `primary`, `secondary` or `accent` (set `--c`).

**Specs** track 6px `border`, radius 3px; fill gradient hue 60%→100%; thumb 20px in the hue with a 6px `bg` core; value in JetBrains Mono 12px in the hue; spring 400/40. Pointer-drag with capture.

*Hand-written from DesignSystemV3.tsx `LiquidSlider`.*
