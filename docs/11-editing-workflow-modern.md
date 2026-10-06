# 11 — Modern Editing Workflow (2026, AI‑assisted) for a Phase‑1 video

How to actually edit one of these "vertical scroll" videos today, using current + AI
tools. The *look* is still the one in `docs/09`; this file is the *how‑to pipeline*.

> Golden rule stays: AI speeds up production, but **you fact‑check every number** and you
> keep the edit clean. AI makes assets, not decisions.

## The 7‑step pipeline

```
1 SCRIPT → 2 VOICEOVER → 3 ASSETS → 4 ASSEMBLE (scroll) →
5 TEXT + SFX + MUSIC → 6 CAPTIONS + POLISH → 7 EXPORT + THUMBNAIL
```

### Step 1 — Script (with `[SHOW:]` cues)
- Write it with `templates/script-template-ladder.md` (or `prompts/03-script-writer.md`).
- Every line already has a `[SHOW: …]` cue → that becomes your shopping list for assets.
- **Fact‑check every number.** Save sources for the pinned comment.

### Step 2 — Voiceover (VO)
Pick ONE:
- **AI voice (fastest):** ElevenLabs, Play.ht, or Murf — pick a calm documentary male/
  female voice, export MP3. Great for faceless + consistency.
- **Your own voice:** any decent USB mic (e.g. a cheap condenser) in a quiet room.
- Clean it: in your editor or Adobe Podcast "Enhance" (free) to remove noise.
- **The VO is your timeline's backbone** — everything else syncs to it.

### Step 3 — Gather / generate ASSETS (from your `[SHOW:]` list)
For each cue, get one visual:
- **Icons / silhouettes:** Flaticon, The Noun Project (divers, animals, submarines, buildings).
- **Real photos:** Pexels, Unsplash, Wikimedia (wrecks, mountains, space).
- **Stock video clips:** Pexels Video, Pixabay, Storyblocks (optional breathers).
- **AI images (for things stock can't give):** Midjourney / Leonardo.ai / Flux / Ideogram
  — e.g. "deep‑sea anglerfish in pitch black, cinematic, dark" . Keep ONE consistent
  style across the video (same prompt suffix) so it looks branded.
- **AI video clips (optional, for wow moments):** Runway, Kling, or Sora‑style tools —
  short 3–5s clips (a descent, an explosion). Use sparingly.
- Put everything in one folder named per depth/step (`01_surface`, `02_40m`, …).

### Step 4 — Assemble the SCROLL (the core technique)
Software: **CapCut (easiest, free)** or **DaVinci Resolve (free, more control)**.
1. Drop the **VO** on the timeline first.
2. Build a **tall vertical gradient background** (bright at top → dark → black at the
   "scary"/extreme zone). In CapCut use a gradient image; in Resolve use a gradient
   generator on a tall canvas.
3. Place each milestone's **label box + object** down the vertical axis at the moment the
   VO says it.
4. Create the "diving/zooming" feel by **keyframing the Position (Y)** of the whole stack
   so it scrolls at a steady speed. (Zoom‑out videos: keyframe Scale instead.)
5. Anchor each object at its depth; let old ones slide off the top as new enter the bottom.
6. **Sync tightly:** the visual for a fact must land within ~1s of the VO saying it.

### Step 5 — TEXT + SFX + MUSIC
- **Text:** bold sans‑serif (Montserrat Bold / Impact), white with a thin dark outline.
  Numbers/labels **pop or slide in from the left**; tone shifts fade in slowly.
- **SFX:** subtle whoosh/thud when boxes/icons slide in (Pixabay, YouTube Audio Library).
- **Music:** one ambient/mysterious synth bed, low volume, ducked under the VO (CapCut/
  Resolve auto‑ducking). Sources: YouTube Audio Library, Pixabay, Epidemic Sound.

### Step 6 — CAPTIONS + polish
- **Auto‑captions:** CapCut "Auto Captions" (or Resolve) → burn in stylish subtitles.
  Big share of viewers watch muted → captions lift retention.
- Watch the **first 30 seconds** like a hawk: fastest cuts, strongest visual, no dead air.
- Check pacing: a visual change every **5–8 seconds**. Trim anything that drags.

### Step 7 — EXPORT + THUMBNAIL
- Export **1080p (or 4K) MP4, H.264**.
- Thumbnail (`docs/04`): make in Canva / Photopea (free) / Photoshop; add an AI‑generated
  hero image if useful. Big subject + ≤4 bold words + high contrast. Do the shrink test.
- Upload with the title (`docs/02` Phase‑1 formulas) + description
  (`templates/description-template.md`) + pinned sources comment.

## Realistic time + cost (solo, with AI)
| Step | Time | Cost |
|---|---|---|
| Script + fact‑check | 3–5 hrs | free (AI draft) |
| Voiceover | 30–60 min | ElevenLabs ~free–$5/mo tier |
| Assets | 2–4 hrs | mostly free (+ optional Midjourney ~$10/mo) |
| Assemble + text + music | 4–8 hrs | free (CapCut/Resolve) |
| Captions + polish + thumbnail | 1–2 hrs | free |
| **Total** | **~1.5–2 days** | **~$0–20/mo of tools** |

## The toolkit (quick list)
- **Edit:** CapCut (start here) or DaVinci Resolve (free).
- **Voice:** ElevenLabs / your mic + Adobe Podcast Enhance.
- **Images:** Pexels, Unsplash, Flaticon + Midjourney/Leonardo/Ideogram.
- **AI clips (optional):** Runway / Kling.
- **Music/SFX:** YouTube Audio Library, Pixabay, Epidemic Sound.
- **Thumbnail:** Canva / Photopea / Photoshop.
- **Captions:** CapCut Auto Captions.

> When you later move to Phase 2 (map‑essays), add the heavier map stack from `docs/05`
> (After Effects + GEOlayers 3 + MapTiler). For Phase 1 you don't need any of that.
