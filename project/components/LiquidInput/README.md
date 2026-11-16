# LiquidInput

Text field whose focus draws a liquid cyan→violet line along its bottom edge.

**Consumer provides** `label` (uppercase micro-label), `value`/`onChange`, `type`, an optional leading Lucide icon (16px), an optional trailing node (e.g. show-password), `placeholder`, `error` text.

**Specs** fill `bg-2`, border 1.5px `border` → `primary-focus` on focus → `error` at 31% on error; `radius-md`; DM Sans 14px; left padding 42px with icon. Label and icon turn `primary` on focus. Focus line: 2px, gradient `primary`→`accent`, scales in from the left over 0.35s with a 5px cyan drop-shadow. Error text 11px `error`, fades in from 3px above.

*Hand-written from DesignSystemV3.tsx `LiquidInput`.*
