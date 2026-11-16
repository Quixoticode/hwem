# LiquidCard

Liquid glass: a translucent card that floats over the background blobs and lifts on hover, catching cyan light.

**Use** for feature tiles, product cards and marketing content over the animated background. Inside dense product UI use the flat `bg-2` panel instead.

**Consumer provides** the content; the card needs something behind it (blobs, the neural canvas) for the blur to read.

**Specs** fill `glass`, `backdrop-filter: blur(blur-glass)`, border `glass-border`, `radius-glass`; hover translateY(-4px), border `rgba(0,240,255,.3)`, shadow `glass-hover`; easing `cubic-bezier(.16,1,.3,1)` 0.4s. Headline words may use `.nl-text-liquid` (cyan→amber at 135°, padding-bottom .1em so descenders aren't clipped).

*From the brand guide §5.1 and §5.3.*
