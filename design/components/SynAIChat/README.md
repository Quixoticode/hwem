# SynAIChat

SynAI's chat window: the product's main conversational surface — it thinks visibly, then streams its answer character by character.

**Anatomy** header (avatar, name, live status, expand/close) · message log · suggestion chips (only while the conversation has fewer than 3 messages) · composer (input + small primary send button).

**Consumer provides** the message list (`role` ai | user, `text`, `state` complete | thinking | streaming), the send handler, suggestions, and the status line.

**Specs** window `bg-2`, `border`, `radius-2xl`, 520px high in the source; header `surface` with 16/20 padding. AI bubble `surface` + `border`; user bubble `accent` at 9% fill / 25% border; both 12/16 padding, `body-sm` at 1.65, `radius-xl` with a `radius-tag` tail corner toward the sender. `**bold**` in AI replies renders in `primary`. Messages rise 10px on a 400/30 spring. Streaming: 18 ms per character with a 2×14 `primary` caret blinking at 0.7s. Thinking: see ThinkingBubble, 1.8–3 s. Avatar: 38px `radius-md`, cyan→violet 13% tint with the xSyna mark at 22px; the user avatar is a 32px `accent` initial tile.

**Do** keep the status line in `success` with a breathing 6px dot. **Don't** stream system errors — show them instantly.

*Hand-written from DesignSystemV3.tsx `SynAIChat`, `SynAIAvatar`, `StreamingText`; the preview is interactive (type, send, watch it think and stream).*
