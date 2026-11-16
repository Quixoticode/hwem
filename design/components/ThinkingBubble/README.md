# ThinkingBubble

SynAI's thinking state: a pulsing 4×2 neural grid above a rotating status line, next to a glowing avatar.

**Use** between a user message and the first streamed character. Rotate the labels every 1.2 s: "Analyzing neural patterns…", "Processing your request…", "Searching knowledge base…", "Generating response…".

**Specs** bubble `surface` with a `primary` 19% border, max 300px; grid cells 18px high, radius 3px, `primary`→`accent` at 38%, each pulsing opacity .2→1 and scaleY .3→1 over 0.9 s with 0.1 s stagger; label `mono` 12px `muted`. Avatar glows 0→20px `primary` and throws a halo ring every 1.5 s.

*From DesignSystemV3.tsx `ThinkingBubble`.*
