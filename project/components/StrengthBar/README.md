# StrengthBar

Four-segment password strength meter under a password field.

**Rule (from source)** empty → hidden · under 6 chars → Weak (`error`) · under 10 → Fair (`secondary`) · 10+ → Good (`secondary`) · 10+ with a symbol → Strong (`success`).

**Specs** segments 3px high, radius 2px, gap `space-4`, empty `border`; label `micro` in the level's colour. Segments fill left to right with 50 ms stagger.

**Note** Fair and Good share amber in the source — the label text carries the difference, so always show it.

*From DesignSystemV3.tsx `StrengthBar`.*
