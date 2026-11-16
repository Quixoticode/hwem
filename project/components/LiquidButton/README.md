# LiquidButton

The filled action button: a diagonal gradient of its hue, a soft glow, and a ripple that spreads from the exact contact point.

**Use** `primary` for the one main action per view, `ghost` beside it for the alternative, `secondary`/`accent` for highlights and features, `danger` for destructive steps, `success` for confirmations.

**Consumer provides** the label (optionally a Lucide icon at 15–17px before or after it), `variant` (primary · secondary · accent · success · danger · ghost), `size` (xs 30px · sm 36px · md 48px · lg 60px high), `disabled`, `fullWidth`.

**Specs** `radius-md`; Space Grotesk 600, +0.02em; padding xs 5/12 · sm 8/16 · md 12/24 · lg 16/40; gradient 130° from the hue at 93% to 60%; shadow `glow-primary` in the variant's hue; hover scale 1.02, press 0.963 (spring 500/28); ripple 70px disc growing ×7 over 0.75s; disabled `opacity-disabled`. Loading: a 14px ring spinner before the label.

**Don't** put white text on `success`, `secondary` or small `danger` buttons in new work — they fail contrast (the V3 source does; the preview keeps it). Use `bg` text there.

*Hand-written from DesignSystemV3.tsx `LiquidButton`; static CSS rendition, ripple via a tiny script.*
