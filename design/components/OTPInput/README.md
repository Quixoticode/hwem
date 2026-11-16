# OTPInput

Six-cell verification code where each digit falls in on its own.

**Consumer provides** `value` (digits only, max 6) and `onChange`; a hidden numeric input carries focus.

**Specs** cells 46×54, radius 11px, gap `space-8`; empty `bg-2` + `border`; active cell 27% `primary` border, scale 1.07, blinking 2×20 cursor; filled 60% `primary` border, 5% fill, digit drops in from −14px.

*Hand-written from DesignSystemV3.tsx `OTPInput`.*
