# LiquidBackground

The ambient layer behind every page: three blurred colour blobs slowly morphing their shape.

**Consumer provides** nothing — place it fixed, `inset:0`, `pointer-events:none`, behind content (`z-index:0`, content at 1).

**Specs** blobs `primary` at 12% (700px), `accent` at 9% (600px), `secondary` at 7% (500px), each blurred to ≈19% of its size, morphing border-radius over 22 s / 28 s / 20 s. Landing pages may swap or add the Three.js neural canvas from the brand guide. Drop the animation under reduced motion.

*From DesignSystemV3.tsx `BgBlobs`; hex-alpha colours kept from source.*
