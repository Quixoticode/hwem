# LiquidToggle

On/off switch with a spring-driven thumb and a cyan glow when on.

**Consumer provides** `checked`, `onChange`, optional `label` (13px `muted`). Render as `role="switch"` with `aria-checked`.

**Specs** track 44×24, `radius-md`, off `bg-2` + `border`; on: `primary` at 15% fill, 33% border, 16% glow. Thumb 16px, off `muted` at x=2, on `primary` at x=21 with `glow-dot` (spring 600/32).

*Hand-written from DesignSystemV3.tsx `LiquidToggle`.*
