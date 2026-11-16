# Loading

How Neuromorphic Liquid waits. Every wait is a small biological process — never a generic spinner — and the motion tells the user *what* is happening, not just *that* something is.

## Pick by duration

| Wait | What to show |
| --- | --- |
| under 300 ms | nothing — avoid the flash |
| 300 ms – 2 s | an inline loader in the control itself (button spinner, `think` dots) |
| 2 – 10 s | a loader from the table below **plus** a mono status line ("Searching knowledge base…"), rotated every 1.2 s |
| over 10 s or known size | a determinate loader with % in `mono` (`load`, `download`, Liquid fill) and, if possible, a step log like `bootup` |
| first paint of content | Liquid skeleton in the shape of the content, never a centred spinner |

## Pick by moment

| Moment | Loader | Hue |
| --- | --- | --- |
| SynAI is composing an answer | Think dots / ThinkingBubble | cyan |
| Model inference on the xSyn chip | Spike train | cyan + one amber spike |
| Searching memory or the knowledge base | Echo search | cyan, amber "hit" |
| Writing to memory, saving notes | Consolidate | violet |
| Training, learning a new skill, indexing files | Mesh weave | cyan, amber hub |
| Spawning, forking or cloning an agent | Mitosis | cyan → violet |
| Pairing a device, joining the collective | Synapse link | cyan ↔ amber |
| Live connection established / streaming | Connect | green |
| Background sync | Sync | cyan + amber |
| Sending a message or file | Send | cyan |
| Uploading / saving with known progress | Liquid fill | cyan → violet |
| Receiving a download | Download | amber |
| Heavy computation, batch jobs | Process | violet |
| System health check, diagnostics | EEG scan | green |
| Listening to voice input | Voice cortex | cyan → violet |
| Encrypting, processing privately on-device | Privacy seal | amber |
| App launch, splash screen | Mark draw (then Bootup log for long starts) | brand gradient |

## Colour meaning while loading

- **Cyan (`primary`)** — electric, the system working.
- **Amber (`secondary`)** — human, private or collective: your data, your devices, other SynAIs.
- **Violet (`accent`)** — memory and learning.
- **Green (`success`)** — live and healthy. Never use it for "busy".
- **Red (`error`)** never animates; a failed load stops and says why.

## Motion rules

- Loops between 1.1 s and 2.8 s; nothing faster than 0.7 s (it reads as alarm).
- Ease with `cubic-bezier(.65,0,.35,1)` for back-and-forth motion and `cubic-bezier(.16,1,.3,1)` for things that emerge.
- One loader per region. If several things load, show the slowest one and list the rest in the mono status line.
- Finish with a beat: the last frame resolves (nucleus pops, ring closes, "READY ✓") before content fades in with the 0.32 s screen transition.
- Under `prefers-reduced-motion`, show the static final frame plus the status text.

## Writing the status line

Mono, sentence case, present progressive, ending in `…`: "Weaving knowledge mesh…", "Sealing on-device…", "Linking to collective…". Finished states in UPPERCASE with a check: `SYNCED ✓`, `READY ✓`.
