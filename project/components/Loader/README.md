# Loader

The loader family: one animation per moment in the neural lifecycle — think, sync, send, load, bootup, process, download, connect.

**Use** `think` while SynAI composes · `sync` for background syncs · `send` while a message or file leaves · `load` for determinate progress with % · `bootup` for system start (mono log) · `process` for heavy computation · `download` for incoming data (amber) · `connect` for establishing a live link. More moments: see LoaderConcepts.

**Specs** cards `bg-2`, `border`, `radius-xl`, 24/20 padding, label Space Grotesk 600 12px uppercase `muted`, hover border `primary-line`. think: three 10px `primary` dots bob 10px, 1.2 s, 0.2 s stagger · sync: counter-rotating 2.5px arcs (`primary` 2 s, `secondary` 2.5 s) around a glowing core · send: send icon flies across with a fading trail, 1.8 s · load: 6px track, `primary`→`accent` fill, mono % in `primary` · bootup: 9px mono lines prefixed "> ", last "READY ✓" in `success` · process: 8 `accent` dots on a ring fading in sequence (1 s) around a 3 s spinner · download: amber icon dropping 12px over a 4px amber bar · connect: pulsing `success` dot + five equaliser bars.

*Hand-written from DesignSystemV3.tsx `LoaderCard`.*
