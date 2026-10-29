# 9:16 Shorts Episode Template

**Goal:** a vertical historical micro-documentary **under 60 seconds**, aiming for 50–55 seconds. Copy this for each episode.

## Brief

- Topic:
- Short title:
- Hook type (contrast, misconception, failed attempt, unexpected consequence):
- Opening line (first 1–3 seconds):
- Central question and promised answer:
- Main causal chain:
- Narrator / voice:
- Target length: 53 seconds
- Format: 9:16 portrait

## Verified fact ledger

| ID | Claim | Year/period | Location | Reliable source | Confidence |
|---|---|---|---|---|---|
| F01 | | | | | |
| F02 | | | | | |

## Micro-story and script

| Time | Function | Exact narration | Visual |
|---|---|---|---|
| 0:00–0:03 | Pattern interrupt | | |
| 0:03–0:10 | Mystery and rewind | | |
| 0:10–0:24 | Origin/problem | | |
| 0:24–0:39 | Pivotal changes | | |
| 0:39–0:48 | Present-day answer | | |
| 0:48–0:53 | Subscribe, future-topic comment, sign-off | | |

Aim for ~105–130 spoken words, adjusted to the measured voice speed. No mid-video subscription interruption. The final CTA must follow the payoff.

## Voiceover preservation

Follow [VOICEOVER_SCRIPT_POLICY.md](VOICEOVER_SCRIPT_POLICY.md). Before narration generation, save the exact script as `episodes/<episode-id>/voiceover-script.md` and record the narrator, version, duration, and asset references in `episodes/<episode-id>/voiceover-metadata.md`. Verify the saved script matches the TTS input. For alternate voices, retain the script and save each audio take separately. Do not overwrite previous takes.

- Episode ID:
- Script version:
- Canonical script path:
- Selected narrator:
- Generated audio take / project reference:
- Measured narration duration:
- Alternate take references:

## Visual masters

Follow [STICKMAN_WARDROBE_GUIDE.md](STICKMAN_WARDROBE_GUIDE.md).
- Character identity and stable face:
- Hat / shirt / vest or jacket / trousers or shorts / footwear:
- Outfit colors, materials, accessories:
- Featured object designs for each era:
- Environment and era:
- Mobile UI-safe framing and text placement:

## Shot record (repeat 6–10 times as appropriate)

- Shot ID / target seconds / actual seconds:
- Exact narration / fact IDs / year:
- Character, outfit, object, and environment masters:
- Starting pose and position:
- Action and object interaction:
- Ending pose and transition:
- Camera, light, and portrait composition:
- Date label or other on-screen text:
- Full 9:16 image prompt:
- Visual-only motion prompt:
- Generation job/status and QA:

## Audio policy

Use [NARRATOR_ONLY_AUDIO_POLICY.md](NARRATOR_ONLY_AUDIO_POLICY.md) for every shot. The designated narrator is the only intelligible voice. Append the silent-scene prompt suffix to every motion/video prompt. Mute generated clip source audio if separate from narration. Confirm no dialogue, crowd chatter, or duplicate narrator before export.

## Pre-export checklist

- [ ] Strong truthful first 1–3 seconds; no generic intro
- [ ] 2–4 meaningful, verified milestones; clear causality
- [ ] All assets composed in portrait 9:16
- [ ] Stickman characters retain period clothing and identity
- [ ] Captions and action readable within mobile safe area
- [ ] Ending answers the opening mystery
- [ ] Brief subscribe + comment invitation only at end
- [ ] Narration aligned and audible; no clipped ending
- [ ] **Measured runtime strictly under 60 seconds**
- [ ] Saved/exported result verified; public publishing not assumed
