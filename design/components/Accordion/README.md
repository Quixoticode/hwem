# Accordion

Collapsible settings group tinted by its section colour when open.

**Consumer provides** `title`, `sub`, the body content, and a `color` (`primary`, `secondary`, `accent`) via `--c`.

**Specs** `radius-md`, `bg-2`, `border`; open: border hue 27%, fill hue 2%, title in hue; header 16/18 padding, title Space Grotesk 600 14px, sub 12px `muted`; chevron rotates; body height animates with spring 300/30.

*Hand-written from DesignSystemV3.tsx `AccordionItem`; the CSS rendition uses `<details>`.*
