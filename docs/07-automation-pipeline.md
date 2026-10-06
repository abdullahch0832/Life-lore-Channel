# 07 — The Automation Pipeline (end‑to‑end factory)

The goal: ship **1 high‑quality video per week** with you + AI + one editor. This is the
assembly line that ties every other module together.

## The 6 stations

```
 ┌──────────────┐   ┌──────────────┐   ┌──────────────┐
 │ 1. MINE      │ → │ 2. PACKAGE   │ → │ 3. SCRIPT    │
 │ ideas+outliers│   │ title+thumb  │   │ write+factcheck│
 │ (NexLev)     │   │ FIRST        │   │ (AI+human)   │
 └──────────────┘   └──────────────┘   └──────┬───────┘
                                              ↓
 ┌──────────────┐   ┌──────────────┐   ┌──────────────┐
 │ 6. LEARN     │ ← │ 5. PUBLISH   │ ← │ 4. PRODUCE   │
 │ log + iterate│   │ + describe   │   │ VO+map edit  │
 └──────────────┘   └──────────────┘   └──────────────┘
```

### Station 1 — MINE (½ day, batched monthly)
- Run the NexLev weekly routine (`docs/08`) → add 15–20 ideas to the backlog.
- Each backlog row: topic · chosen formula (F1–F7) · source outlier · demand evidence.
- **Package‑first rule:** never promote an idea past this station without a title that
  scores well on the `docs/02` rubric.

### Station 2 — PACKAGE (before scripting!) 
- Write title (top‑2 variants) + design the thumbnail concept **first**.
- If you can't make a compelling package, the topic dies here. This saves you from
  scripting videos nobody will click. (This is the RealLifeLore discipline: the package
  is the product.)

### Station 3 — SCRIPT (1–2 days)
- Generate draft with `prompts/03-script-writer.md` against the 8‑beat skeleton.
- **Human fact‑check pass** — verify every stat with a source (`docs/03`). Non‑negotiable.
- Mark [MAP] / [B‑ROLL] cues for the editor.

### Station 4 — PRODUCE (2–3 days)
- Voiceover: your narrator or a TTS you're comfortable with. *(Per your note, voice is
  out of scope for analysis — your choice of VO stands; the system doesn't depend on it.)*
- Edit to the `docs/05` spec: dark map base, GEOlayers moves, stat pop‑ins synced to VO,
  b‑roll breathers, fast pacing.

### Station 5 — PUBLISH
- Fill `templates/description-template.md` (credits, sources, sponsor, links).
- Upload with packaged thumbnail. Title exactly as chosen. Pin a comment with sources.
- Keep tags light/brand‑level (the niche doesn't rank on tags — `docs/01`).

### Station 6 — LEARN
- After 7/28 days, log CTR, avg view duration/%, views, and which formula/thumbnail won.
- Use NexLev `get_my_*` tools (if your channel is connected) for retention & traffic
  sources. Double down on the formulas and thumbnail styles that win; retire losers.

## Suggested weekly cadence (solo + 1 editor)

| Day | Station | Output |
|---|---|---|
| Mon | 1–2 | Idea locked, title + thumbnail concept done |
| Tue–Wed | 3 | Script drafted + fact‑checked + cue‑marked |
| Wed | 4a | VO recorded/generated; thumbnail finalized |
| Thu–Fri | 4b | Map edit assembled to spec |
| Fri | 5 | Publish + description + pinned sources |
| (ongoing) | 6 | Review last video's analytics |

## Where AI plugs in (and where humans must stay)

| Step | AI does | Human must |
|---|---|---|
| Idea mining | Summarize NexLev outliers, cluster themes | Pick what fits brand + formula |
| Titles | Generate all formula variants + score | Choose final 2; sanity‑check honesty |
| Script | Draft 8 beats in‑voice, suggest analogies | **Fact‑check every number**, cut fluff |
| Thumbnail | Draft concepts (NexLev generate/edit) | Final design + shrink/contrast test |
| Description | Fill template | Verify sponsor + source links |
| Analytics | Pull + summarize metrics | Decide strategy changes |

> **Hard rule:** AI never publishes an unverified statistic. The channel's survival is
> its credibility.

## Tooling summary
- **Research/analytics:** NexLev (`docs/08`), Google Trends, Wikipedia/World Bank/OWID.
- **Scripting:** this repo's prompts + an LLM.
- **Edit:** DaVinci Resolve/Premiere + **GEOlayers 3** + MapTiler/Mapbox + stock library.
- **Tracking:** a simple spreadsheet or the `templates/video-brief-template.md` per video.
