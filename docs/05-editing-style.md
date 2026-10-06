# 05 — Editing & Production Style (how to replicate the look)

> You asked specifically to analyze the **editing style**. This is the most detailed
> module. It combines (a) a frame‑level visual analysis of a modern video and (b) the
> **actual toolchain**, which they reveal in their own video descriptions.

## Their real toolchain (confirmed, not guessed)

The description of *"Why 95% of Australia is Empty"* literally credits their tools:

```
Special thanks to MapTiler / OpenStreetMap Contributors and GEOlayers 3
Select video clips courtesy of Getty Images
Select video clips courtesy of the AP Archive
```

So the production stack is:

| Layer | Tool they use | Cheaper/alt options for you |
|---|---|---|
| Animated maps | **GEOlayers 3** (aescripts plugin for After Effects) + **MapTiler / OpenStreetMap** tiles | GEOlayers 3 is the key buy. Free‑ish: Google Earth Studio (3D flyovers), QGIS, `mapbox` |
| Compositing / motion | **Adobe After Effects** | After Effects (standard); DaVinci Resolve Fusion |
| 3D globe flythroughs | Google Earth Studio (very likely) | Google Earth Studio (free) |
| Stock / archival footage | **Getty Images**, **AP Archive** | Storyblocks, Pexels/Pixabay (free), Artgrid |
| Edit / assembly | Premiere Pro / Resolve | DaVinci Resolve (free) |
| Typography | Clean geometric sans (Montserrat‑style) | Montserrat / Inter / Archivo (free) |

**The single highest‑leverage purchase for this style is GEOlayers 3** — it's what makes
the "label a city / draw a route / zoom a region" map animations look professional.

## Frame‑level visual analysis (first 3 minutes of a modern video)

### 1. Maps are the star (~75% of screen time)
- Frequent **zoom + pan** moves across a stylized world map; the "camera" often **flies**
  across the globe to transition between regions instead of hard cutting.
- **Shape/size overlays:** a white‑outlined silhouette of the subject country laid over
  another region for scale comparison, filled with a semi‑transparent color.
- **Density heatmaps:** custom red/blue shaded maps to show population distribution —
  turning a statistic into an instant visual.
- **Red "target" markers** pinpoint cities consistently.

### 2. Footage mix (~25%)
- 4K **aerial/drone** b‑roll (golden‑hour graded) and **street‑level crowd** footage from
  Getty/AP, used as "breathers" to ground abstract data in real places.
- **No talking heads, no archival movie clips** in the base format — purely informational.

### 3. On‑screen data
- Stats appear in **small high‑contrast boxes** (white/black/red) that **pop or fade in
  exactly as the narrator says the number.**
- Clear hierarchy: big bold ALL‑CAPS names, smaller light text for figures.

### 4. Pacing & transitions
- **Fast:** a visual change every **2–4 seconds**. Nothing sits static.
- Map‑to‑map = smooth flythrough; map‑to‑b‑roll = clean **hard cut**.

### 5. Color & tone
- **Dark‑mode maps** (deep blue oceans, high‑contrast land) so white outlines and colored
  overlays pop. B‑roll graded warm/vibrant for contrast with the cool maps.

### 6. Typography
- One clean geometric **sans‑serif**, ALL CAPS headers, text either white‑on‑dark or
  black/white inside a colored rectangle for legibility over busy maps.

### 7. Audio‑visual sync (the retention secret)
- Visuals are **frame‑accurately synced to narration**: narrator says "Java" → map
  highlights Java; "crowded cities" → cut to a packed street. **Every noun the script
  names gets a matching visual within ~1 second.** This tight sync is a huge part of why
  people watch 30+ minutes.

## A replication checklist (hand this to your editor)

- [ ] Dark‑mode base map styled in MapTiler/Mapbox (deep blue sea, muted land).
- [ ] Country/region moves done in GEOlayers 3 (zoom, pan, highlight, route lines).
- [ ] Every stat = a pop‑in box, timed to the exact word in the VO.
- [ ] Every named place = a map highlight or a labelled marker within ~1s.
- [ ] A size‑comparison overlay at least once (subject silhouette vs a known region).
- [ ] One density/heatmap visual for the core statistic.
- [ ] 4K aerial/street b‑roll every ~30–45s as a breather, hard‑cut in, warm graded.
- [ ] Visual change ≤ every 4 seconds; no static holds.
- [ ] Consistent font + lower‑third style (brand lock).
- [ ] Soft neutral documentary music bed; duck under VO.
- [ ] One seamless sponsor segment bridged thematically from the content.
- [ ] Export 4K/1080p, upload with the packaged thumbnail (`docs/04`).

## Realistic "good‑enough v1" version
You don't need their full budget to start. Minimum viable version of this look:
**DaVinci Resolve (free)** + **GEOlayers 3** (the one paid plugin) + **free stock
(Pexels/Pixabay)** + **Montserrat** + **dark Mapbox style**. That reproduces ~80% of the
perceived quality. Add Getty/Artgrid and Earth Studio flythroughs once revenue allows.
