# Narrator-Only Audio Policy — Shorts

**Default: exactly one intelligible voice in the finished video, the designated narrator.** Stickman characters are silent visual actors. This rule applies to every scene, including crowd scenes, workshops, roads, factories, the hook, and the end card.

## Generation rule

1. Generate a single narration track using the chosen narrator and the exact approved script. Never ask the video model to recite or reenact narration.
2. When the generator supports **Video Only**, **mute generated audio**, **disable dialogue/speech**, or equivalent, choose the supported setting that creates visuals without scene voices. Verify the setting for each job. Do not invent UI controls.
3. If generated clips include sound, mute their **source/clip audio** in the editor before placing the narration track. Optional ambience and instrumental music should be added separately and kept below narration.
4. If VideoExpress has an integrated Narration Video mode, verify whether its generated audio is the narrator track, incidental scene audio, or both. Avoid adding a second narration copy. Preserve the designated narrator while removing only unwanted source dialogue.
5. Do not direct characters to talk, shout, whisper, chant, sing, mouth words, give speeches, or lip-sync. They may point, gesture, react silently, work, and show expressions. Their mouths may smile or change expression but must not articulate words.
6. Do not generate crowd chatter, radio speech, announcements, TV voices, background conversations, or vocal music. For realism, use **non-vocal** environmental sounds only if deliberately enabled.
7. Perform an audio-overlap QA check before export. Listen or inspect the timeline at the beginning, each scene transition, midpoint, and ending. If unwanted voices remain, mute the offending clip source, replace the affected scene with silent visuals, or regenerate only that clip. Do not accept overlapping intelligible speech.

## Mandatory prompt suffix for every video/motion generation

"**SILENT SCENE — VISUALS ONLY.** All on-screen stickman characters are non-speaking performers. They may gesture, point, walk, react, and interact with props, but **no dialogue, speech, whispered words, shouts, singing, lip-sync, talking mouths, background conversations, radio/TV voices, crowd chatter, or extra narrators**. Generate **no vocal audio**. The separate designated narrator track supplies all spoken words. If the video generator supports silent/video-only output, use it."

For image prompts, keep the instruction simple: "Characters are silent visual actors, not speakers." Still apply the full audio policy when animating the image.

## Timeline mixing

| Track | Default | Rule |
|---|---|---|
| Primary narrator | On | Exactly one authorized narration, uninterrupted |
| Generated clip audio | Muted | Prevent model-invented character speech |
| Background music | Optional, instrumental | Quiet enough that every word is intelligible |
| Sound effects | Optional, non-vocal | Brief, purposeful, never competing with narrator |

If source audio and narration are already mixed into one exported stereo track, simple muting removes both. Return to the editor/project and mute the **original scene audio before mixing**. Source separation after export is an uncertain fallback and can introduce artifacts; never promise a clean separation.

## Required QA gate

- [ ] Every scene prompt includes silent-scene instructions
- [ ] Scene audio disabled or source clips muted where supported
- [ ] Exactly one intelligible speaking voice in final mix
- [ ] No characters lip-sync or appear to speak
- [ ] No background crowd/radio/TV voices
- [ ] Narration clear, not duplicated, not cut off
- [ ] Final video remains vertical 9:16 and strictly under 60 seconds
