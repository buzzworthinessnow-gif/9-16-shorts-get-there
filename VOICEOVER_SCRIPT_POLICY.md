# Voiceover Script Preservation and Voice-Swap Policy

Every Shorts production must preserve its **exact approved spoken narration text** as a reusable artifact before generating voice audio. This includes the hook, history, transitions, and closing subscribe/comment invitation.

## Required assets for each episode

Use a stable episode identifier such as `car-origins-short-001` and maintain:

1. `episodes/<episode-id>/voiceover-script.md` — canonical editable script, exact words and punctuation, including pauses and optional pronunciation notes.
2. `episodes/<episode-id>/voiceover-metadata.md` — script version, creation/update date if known, topic, language, selected voice, delivery settings (if available), word count, target/actual duration, generated audio asset IDs or project references, and any known limitations.
3. Optionally `episodes/<episode-id>/voiceover-versions/` for revised scripts, or keep a clearly labeled version history in the canonical script.

**Persistence:** Save the script in the user's current VideoExpress project notes or script field when the UI supports durable saving, and **also save a reusable Markdown copy in the authorized GitHub Shorts repository** when GitHub write access is available. A transient chat response or an unsaved TTS input field does not count as verified preservation. If the account cannot write to GitHub, provide the script as a downloadable file or copyable text and explicitly report that the GitHub copy is not yet saved. Never claim a save without confirming it.

## Before any TTS or video generation

- Complete the fact-check and script; record exact text before submitting to the narrator.
- Assign episode ID and script version (`v1`, `v2`, etc.).
- Save or commit the canonical script and metadata to the episode folder; verify the file exists and content matches.
- Submit **exactly the saved script text** to the selected narrator. Do not rewrite it invisibly when changing voices.

## Changing narrator voice

- Preserve the canonical script. Change only the selected voice and relevant delivery settings.
- Generate a **new labeled voice take**, such as `car-origins-short-001_v1_Beau-Whitaker` or `car-origins-short-001_v1_Alternate-Voice`, and record its project asset reference and measured duration.
- Do not overwrite or delete the original script, prior audio take, or assembled video unless the user explicitly requests it.
- Check the new voice's actual duration; adjust scene timing and maintain a final runtime strictly under 60 seconds. If it does not fit, request approval for a shortened script or create a separate version and preserve the original.
- Reuse existing visual clips where suitable. Keep the narrator as the **only speaking voice**, per [NARRATOR_ONLY_AUDIO_POLICY.md](NARRATOR_ONLY_AUDIO_POLICY.md).

## Recovering from errors

If the audio overlaps with scene voices, is distorted, or has the wrong narrator, return to the saved script and create a clean narrator take. Mute scene audio separately or regenerate only the affected visuals. Do not attempt to recover the exact script by transcribing a flawed mixed-audio export when a verified script copy exists.

## Script file format

```markdown
# Voiceover — <Episode Title>

Episode ID: <id>
Script version: v1
Narrator: <selected voice>
Target duration: 50–55 seconds
Status: Approved / Draft

## Exact spoken narration

<Exact text to send to TTS, including CTA>

## Pronunciation and delivery notes

<Notes not spoken by TTS>

## Revision history

- v1 — Initial narration script
```

**Important:** Episode files are created when producing an actual episode. This guide does not imply that scripts from already completed videos have been recovered or saved retroactively.
