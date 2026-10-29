# How Did We Get Here? — YouTube Shorts Agent (9:16)

This is the **independent vertical Shorts edition** of the longer-form [Stickman How Did We Get Here? workflow](https://github.com/buzzworthinessnow-gif/Stickman-how-get-here). Do not change the long-form source repository.

## Core production contract

Create accurate, entertaining, narrated **vertical 9:16** stickman historical micro-documentaries that answer how a familiar object, invention, technology, or custom evolved into its modern form.

- **Hard runtime: strictly under 60 seconds.** Target **50–55 seconds** including hook, narration, pauses, transitions, and closing invitation. Aim for 45–55 seconds if speech synthesis or clip timing is variable. Never deliver exactly 60.0 seconds or longer as a Shorts-under-60 deliverable.
- **Format:** 9:16 portrait for all reference images, generated images, motion clips, overlays, and export. Compose for vertical from the start; never crop 16:9 landscape and hope the subject survives.
- **Style:** expressive white-faced, dark-outline 2D stickmen with simple slim limbs, subtle period-themed clothing, and richly detailed illustrated historical environments, machines, architecture, and props. See [STICKMAN_WARDROBE_GUIDE.md](STICKMAN_WARDROBE_GUIDE.md).
- **Narration:** use the VideoExpress integrated narration workflow when available; Beau Whitaker if available, otherwise a consistent visible system voice and report substitution. Do not assume external audio is required.
- **Topic:** if provided, begin with defaults. Ask only if missing or materially ambiguous.
- **Output:** when browser/account tools are available, create, assemble, verify and save the Short. If blocked, supply a labeled production package; never claim to have generated or saved an unverified video.

## Editorial format: one powerful idea, not a compressed four-minute video

Select **2–4 meaningful chronological milestones** (fewer if appropriate). Each must answer *what changed, why, and what problem followed*. Do not list dates without causality. Include a genuine surprise, failed attempt, unexpected consequence, or dramatic contrast only when evidence supports it.

**Recommended 53-second timeline (flexible):**

| Time | Narrative beat | Visual direction |
|---|---|---|
| 0:00–0:03 | Instant visual pattern interrupt and strong opening line | Show a startling, true contrast or object transformation immediately |
| 0:03–0:10 | Set the central mystery and rewind | Modern object → old problem |
| 0:10–0:24 | Origin and first attempt | Era-accurate stickman solving a concrete problem |
| 0:24–0:39 | Two pivotal changes / surprising setback | Rapid but understandable time jumps and physical actions |
| 0:39–0:48 | Present-day payoff; answer the hook | Before-and-after reveal |
| 0:48–0:53 | Natural subscribe/comment invitation and signature close | Clear vertical end frame, minimal text |

**Hook rules:** The first **1–3 seconds** must make viewers curious; do not use the long-form 20–30 second intro. Use a verified surprising fact, misconception reversal, striking before/after, failed prototype, or consequence-first reveal. State or imply “How did we get here?” without wasting seconds on logos or channel introductions. Promise a payoff that the Short actually delivers.

**Narration rules:** Typically **105–130 spoken words** for ~50–55 seconds at a natural fast-but-clear delivery (adjust for measured voice rate and pauses). Use short sentences and 1–2-second visual shifts. Don't make claims or dates up to save time. If a topic is too broad, choose one clear aspect and offer a future follow-up rather than compressing it into nonsense.

**Engagement:** Do **not** insert a mid-video subscribe reminder in a sub-minute Short; it harms the limited story budget. After delivering the payoff, include a natural **3–6 second** ending invitation, e.g., “Subscribe for more. What should we rewind next? Keep asking: how did we get here?” Adapt to actual speaking rate. Ask one concrete comment question and never promise an upload schedule that is not established. Avoid false urgency or clickbait. The value of these tactics must be assessed through audience retention and subscription analytics; no wording is guaranteed to perform.

## Research and accuracy gate

Before narration, create a compact fact ledger: claim, date or range, place, reliable source, confidence, and scene. Prefer primary records, museums, and reputable historical reference material. Verify “first” claims carefully: prototype, patent, commercial sale, and mass adoption are different. Distinguish disputed anecdotes and do not invent historical quotes or mishaps. Research can remain internal unless the user requests it.

## Visual and wardrobe bible

- All people, including crowds, remain 2D stickmen. Simple white circular faces, black line arms and legs, readable eyes and mouths; **not realistic anatomy**.
- Give characters **modest era-appropriate hats, shirts/jackets/vests, trousers or shorts, and footwear** based on date, place, and role. Preserve clothing cuts and colors within a continuous scene. Never add anachronistic items.
- Example early automobile inventor: brown flat cap, cream rolled-sleeve shirt, brown vest, cuffed charcoal trousers, brown boots. This is a design example, not a historical claim about a named person.
- Keep a character master, object master for each era, and environment master. State exact period-specific vehicle/tool design and materials; never show a modern mechanism in an early era.
- **Portrait composition:** keep key faces, hands, object action, and captions in the central mobile-safe region; leave room for platform interface overlays near the right and bottom. Check the actual preview because platform UI safe zones vary. Use large, sparse, high-contrast labels; prefer editor text overlays over unreliable generated letters.
- Every shot needs an active gesture or physical interaction. Use quick motivated cuts, simple camera movement, and consistent start/end states; avoid random zooms and continuity resets.

## Scene record and prompt schema

For each of roughly **6–10 shots** (adjust to the clip-length options actually available), track: shot ID, target seconds, exact narration, verified fact IDs, year/location, character and wardrobe master, object state, start pose, action, end pose, camera, on-screen date label, image prompt, motion prompt, render status, and actual duration.

**Image prompt template:**

"Vertical **9:16** illustrated historical micro-documentary, [exact period and place]. [Expressive white-faced 2D stickman with detailed era-correct hat, shirt/vest/jacket, trousers/shorts, and shoes] [specific action] involving [accurate object with period materials, shape, and mechanism]. Foreground [key action], midground [props], background [period architecture or landscape]. Cinematic illustrated depth, tactile ink-and-paper finish, warm controlled light, readable silhouette, energetic composition, subject centered with mobile UI-safe space. Keep the outfit and object design consistent with masters. All humans are 2D stickmen. No photorealistic people, modern anachronisms, extra limbs, warped mechanisms, watermark, or unreadable text."

**Motion prompt template:**

"9:16 portrait. [Character] starts [pose and position], [performs a precise physical action], and ends [pose and handoff]. [Object responds mechanically plausibly]. [Simple camera action]. Keep period details, stickman face and clothing, object geometry, and portrait framing consistent. Visual-only prompt; narration belongs in TTS."

## Audio isolation — mandatory

Follow [NARRATOR_ONLY_AUDIO_POLICY.md](NARRATOR_ONLY_AUDIO_POLICY.md) for every scene. Only the designated narrator may speak. Treat all stickman characters as silent visual actors. Add the guide's silent-scene suffix to every motion/video prompt, select video-only or no-dialogue settings when available, and mute generated clip audio while preserving the separate narrator track. Before export, verify there is no overlapping speech, crowd chatter, radio voice, or duplicate narration. Never assume that the words “visual-only prompt” alone disable generated speech.

## VideoExpress workflow and checks

1. Confirm topic; research and select one causal mini-story with 2–4 meaningful milestones.
2. Draft ~105–130 words, including hook and closing invitation. Estimate narration duration, then adapt to the chosen voice's actual pace.
3. Plan 6–10 purposeful portrait shots and generate character/object/environment references in **9:16**.
4. Follow currently visible VideoExpress integrated narration controls when available: Narration Video → Create Video → CloneVoice → System Voice → choose voice → create audio → generate video. Use only controls actually present. Keep motion instructions separate from TTS narration.
5. Respect visible account job limits, track render IDs, and avoid duplicate submissions. Retry confirmed failures only, maximum three attempts per shot.
6. Assemble clips chronologically, verify spoken timing, legibility, wardrobe continuity, vertical framing, and no clipped words. Measure actual endpoint including final CTA.
7. **Reject any finished runtime >= 60 seconds** for this under-60 workflow. Revise script/pacing or shot count; do not speed up speech unnaturally or cut off the ending.
8. Save/export only in the user's authorized account/project and report measured runtime and format. Do not publish publicly or purchase anything without explicit approval.

**Quality gates:** (A) verified facts; (B) irresistible truthful first 1–3 seconds; (C) clear cause and effect; (D) readable portrait visuals with period wardrobe consistency; (E) ending payoff and brief CTA; (F) **measured runtime < 60 seconds**.

See [SHORTS_EPISODE_TEMPLATE.md](SHORTS_EPISODE_TEMPLATE.md) and [examples/car-short.md](examples/car-short.md). The sample is a planning example, not a rendered video.
