Neuromorphic Liquid is the visual language of **xSyna** and its products (SynAI, xSyn). The brain is organic, fluid, reactive and adaptive — so is the interface. No rigid grids, no neon-on-pure-black cyberpunk: deep midnight space, bio-luminescent light, and surfaces that behave like liquid.

## Principles

1. **Organic depth.** Never pure black. Build depth on Deep Cortex (`bg`), layer `bg-2` panels and `surface` popovers on it, and let blurred colour blobs drift behind.
2. **Reactive physics.** Everything answers the user: buttons ripple from the touch point, toggles and tabs move on springs, cards lift and catch light, inputs grow a liquid line on focus.
3. **Atypographic symbolism.** Marks and glyphs are clean vector curves that behave like dividing cells or synapses — the xSyna X is two curves around a nucleus.
4. **Three core hues, cognitive focus.** Cyan for impulses and action, amber for the human and collective, violet as a rare third. Status colours stay small.

## Content fundamentals

- Product UI copy is **English**, short and technical-poetic: "Liquid by nature.", "Every interaction breathes. Every component flows.", "Analyzing neural patterns…". Brand and concept docs are written in **German**, in the first person plural ("Wir nutzen…").
- Borrow from neuroscience for names: Cortex, Synapse, Axon mesh, Pulse, Neural sync, Auto-learn. Don't overdo it in functional labels — "Email", "Password", "Settings" stay plain.
- Headings in sentence case; field labels, panel captions and overlines in UPPERCASE with wide tracking.
- Numbered section overlines: `01 / INTERACTIONS` in `overline` mono, `primary`.
- Machine voice (logs, boot lines, metrics) goes in JetBrains Mono, uppercase: `INIT NEURAL CORE v3.2`, `READY ✓`.
- Ellipsis character `…` for in-progress states. No emoji; the only glyphs are `✓`, `→`, `∞`, `×`.

## Colour

- Ground is `bg` (#020407). The brand guide's `cortex` (#030508) is the same idea one step lighter; use `bg` in new product work.
- Stack: `bg` → `section-alt` bands → `bg-2` panels/inputs → `surface` for menus and chat bubbles. Separate with the `border` hairline, never with heavy shadows.
- `primary` (Synaptic Cyan #00e5ff in V3; the guide and trailer use `cyan-500` #00f0ff) marks action, focus, selection and links. Selected things get `primary-tint` fill + `primary-line` border + `primary` text.
- `secondary` (Neural Amber) is the warm counterweight: accents, warnings, human aspects. `accent` (violet) appears in gradients' far end, the user avatar and the security group.
- The cyan→amber gradient (135°) is reserved for the logo and one key word in a hero headline (`.nl-text-liquid`). Cyan→violet (90°) is the input focus line and progress fill. Nothing else gets a gradient except button fills of one hue.
- Background blobs: three 500–700px discs in `primary` (12%), `accent` (9%) and `secondary` (7%), blurred to ~19% of their size, morphing over 20–28s.
- **Themes:** Deep Cortex (`dark`) is the default. Midnight Bio swaps in a violet primary and cyan secondary on navy; Bioluminescent a green primary on deep forest. Only the grounds, text, muted and primary family change — accent, success and error stay. Use the alternates for product or user choice, never mixed on one screen.
- **Contrast:** `text` on every ground passes AAA. `muted` (#4a6080) is only ≈3.2:1 on `bg` — fine for icons and 24px+ text; for small secondary copy that must be read, prefer `text` at reduced emphasis or lift muted in a future revision. White labels on `success`, `secondary` and small `error` fills fail; use `on-primary`/`bg` there.

## Typography

- **Space Grotesk** (`--font-display`) for headlines, buttons, labels, navigation — weights 300–700. **DM Sans** (`--font-body`) for running text. **JetBrains Mono** (`--font-mono`) for code, telemetry, logs, metrics and slider values. All three load from Google Fonts.
- Headlines scale fluidly: `hero` clamp(38, 7vw, 78) at −0.02em, `section-title` clamp(26, 4vw, 42), `display`/`heading-1`/`heading-2` as their usage notes give.
- Body `body` 16px/1.6, sub-copy in `muted` capped at ~520px wide. Labels `label` 11px/700/+0.1em uppercase.
- The original brand guide specified Plus Jakarta Sans; V3 replaced it with Space Grotesk + DM Sans. Use the V3 pair.
- Always enable antialiasing on `body` (`-webkit-font-smoothing: antialiased`).

## Spacing, radii, layout

- Content column max 1100px, gutters `space-24` (16px under 768px). Sections pad `space-80` vertically (52px on mobile), alternate sections sit on `section-alt` with `border` top and bottom.
- Panels pad `space-22`; grids gap `space-24` (two-column), `space-16` (cards), `space-12` (icons). Collapse to one column under 768px.
- Radii are soft and generous, never sharp: `radius-md` (12) for controls, `radius-lg` (14) panels, `radius-xl` (16) nav and bubbles, `radius-glass` (24) Liquid Cards, `radius-pill` for the Bio-Button and dots. Chat bubbles keep one 4px "tail" corner toward their sender.

## Motion

Motion is the brand. Use springs, not linear tweens, for state changes.

- Press: scale 0.963, hover 1.02 (spring stiffness 500, damping 28). Toggles 600/32, tabs and dropdowns 400/28–30, side nav width 400/36.
- Screen transitions: fade + 12px slide + 4px blur, 0.32s `cubic-bezier(.4,0,.2,1)`.
- Glass and reveals: `cubic-bezier(.16,1,.3,1)` — card lift 0.4s, scroll reveal 1s from 40px below.
- Ripples 0.75s ease-out; loaders loop 1.1–2.8s — which loader for which moment is in the Loading section.
- Honour `prefers-reduced-motion`: drop ripples, blobs and loops, keep instant state changes.

## Elevation & effects

- Glow, not shadow: interactive fills carry `glow-primary` in their own hue; active dots `glow-dot`.
- Real drop shadows only for floating layers: `popover` on menus, `glass-hover` on lifted Liquid Cards.
- Glass = `glass` fill + `blur-glass` backdrop blur + `glass-border`.
- Landing pages may add the reactive WebGL neural canvas (Three.js particle network with fog in the Cortex tone) fixed behind everything, `pointer-events: none`.

## Iconography

- **Lucide** icons, outline, stroke 1.5–1.6 (2–3 only inside small buttons and checks), sizes 15–18px in controls, 26px in icon grids. Inactive `muted`, active or hovered in the item's hue with a 1.18 spring scale.
- Concept glyphs in use: Brain (Cortex), Waves (Pulse), Droplets (Liquid), Zap (Energy), Network (Synapse), Cpu (Process), Shield (Secure), Layers (Depth), Orbit, Activity (Vitals), Database (Memory), Sparkles.
- The xSyna mark is in `assets/Logos/` — self-coloured SVG for dark grounds only. Draw it inline when it must animate (the hero radiates eight cyan axon lines from it).

## Components

Liquid Button, Bio-Button, Liquid Card, Liquid Background, Liquid Input, OTP Input, Strength Bar, Toggle, Checkbox, Slider, Chip, Icon Cell, Section Label, Tab Bar, Dropdown, Accordion, Side Nav, the Loader family and the Loader Concepts. Two patterns compose them: the SynAI Chat (with its Thinking Bubble) and the Auth Flow (xSyna SSO). Each has guidelines and a preview under Components; styles live in `components/bundle.css` (classes prefixed `nl-`). The previews are hand-written CSS renditions of the React/framer-motion originals — springs are approximated with CSS easing.

## Not synced

- No React bundle: the source components depend on framer-motion and live inside one demo file; previews are hand-written CSS/JS renditions.
- Fonts are Google-hosted, so no font files are stored.
- The V3 dropdown names a fourth theme, "Neural Void", that has no values anywhere in the code — not added. The first mockup's own "Dark Cortex" (#030508 / #0a0f1a) is superseded by V3's Deep Cortex and kept only as the `cortex` token.
- The trailer's `index.css` (Space Grotesk-only, cyan/amber, text-muted = amber) is a video-specific palette and not merged.
- Loader Concepts and the Loading section are new design work, not extracted from the code.
