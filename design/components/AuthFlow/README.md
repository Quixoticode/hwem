# AuthFlow

The xSyna SSO pattern: one card that walks through Login → Sign Up → Verify → Profile, built only from system components.

**Screens** Login (email, password with show toggle, Remember me toggle, Forgot password link, primary Sign In, divider, Google/GitHub ghost buttons) · Sign Up (name, email, password + StrengthBar, Terms checkbox) · Verify (icon tile, OTPInput, resend countdown in mono, Back) · Profile (avatar with verified badge, PRO badge, three stat tiles, settings list with toggles, ghost Sign Out in `error`).

**Consumer provides** the auth handlers; the card itself is presentational.

**Specs** card `bg-2`, `border`, `radius-sso`, padding `space-28`, faint 60px `primary` glow; brand block: xSyna mark 34px + "XSYNA SSO" 10px/700/0.2em. Screen titles 22px Space Grotesk 700, subtitles 13px `muted`. Screens change with fade + 12px rise + 4px blur, 0.32s `cubic-bezier(.4,0,.2,1)`. Submitting swaps the label for a spinner + "Signing in…" / "Creating…" / "Verifying…". Stat tiles and the settings list sit on `bg` (one step darker than the card). Step list on the left: rows with `radius-md`, active row 33% `primary` border and a `primary` dot.

*Hand-written from DesignSystemV3.tsx `SSOLogin`, `SSOSignup`, `SSOVerify`, `SSOProfile`; the preview is clickable, and the signup password feeds the strength bar.*
