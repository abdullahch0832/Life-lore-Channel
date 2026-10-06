# Life Lore Channel — Faceless Geography/Geopolitics Video System

A complete, repeatable production system reverse‑engineered from **RealLifeLore**
(7.94M subs, 1.98B views, 504 videos) and the wider map‑essay niche, using NexLev
analytics data.

> **Roman Urdu — Khulasa:** Yeh repo aapke channel ka poora "factory system" hai.
> Isme hai: competitor kaise kaam karta hai, title/script/thumbnail kaise bante hain,
> editing style kaise copy karni hai, ideas kahan se aate hain, aur NexLev se puri
> pipeline kaise automate karni hai. Har file ek module hai — upar se niche parho.
> **Note:** Data analyze kiya gaya hai, **voice nahi** (aapne mana kiya tha). Editing
> style zaroor analyze ki gayi hai.

---

## What this system gives you

| # | Module | File | What it answers |
|---|--------|------|-----------------|
| 1 | Competitor teardown | [`docs/01-competitor-analysis.md`](docs/01-competitor-analysis.md) | How RealLifeLore actually works, its two eras, outliers, numbers |
| 2 | Title engine | [`docs/02-title-formulas.md`](docs/02-title-formulas.md) | The exact repeatable title formulas + a swipe file |
| 3 | Script system | [`docs/03-script-system.md`](docs/03-script-system.md) | The 8‑beat script skeleton + how they write |
| 4 | Thumbnail system | [`docs/04-thumbnail-system.md`](docs/04-thumbnail-system.md) | Thumbnail rules, layout, text, colors |
| 5 | Editing / production | [`docs/05-editing-style.md`](docs/05-editing-style.md) | Their exact toolchain + how to replicate the look |
| 6 | Idea sourcing | [`docs/06-idea-sourcing.md`](docs/06-idea-sourcing.md) | Where ideas come from + the mineable competitor ecosystem |
| 7 | Automation pipeline | [`docs/07-automation-pipeline.md`](docs/07-automation-pipeline.md) | End‑to‑end weekly factory, roles, tools, checklist |
| 8 | NexLev playbook | [`docs/08-nexlev-playbook.md`](docs/08-nexlev-playbook.md) | Step‑by‑step: which NexLev tool to run, when |

### Ready‑to‑use assets

- **Templates** → [`templates/`](templates/) — fill‑in‑the‑blank script, description, and video brief.
- **AI Prompts** → [`prompts/`](prompts/) — copy‑paste prompts to generate ideas, titles, and full scripts in the RealLifeLore style.
- **Data** → [`data/reallifelore-dataset.md`](data/reallifelore-dataset.md) — the raw outlier + benchmark data this system was built from (captured 2026‑10‑05).

---

## The 10‑second mental model

RealLifeLore is **not** "a geography channel." It is a **curiosity‑gap packaging
machine** that happens to use geography as raw material:

```
PICKABLE TOPIC  →  SHOCKING FRAMING (title+thumb)  →  10–50 min "mystery → why" essay
   (country,          "Why 95% of X is Empty"            over animated maps + stock
    conflict,          "What's Hidden Under the Ice"      b-roll, 1 seamless sponsor
    anomaly)           "X's Catastrophic Y Problem"
```

Win the **package** (title + thumbnail promise), deliver a **satisfying mystery‑then‑
explanation arc**, wrap it in a **map‑heavy fast edit**. Everything in this repo is a
tool to do those three things on repeat.

## The two‑phase plan (IMPORTANT — read this)

- **Phase 1 (start here):** remake the OLD short "curiosity / scale / what‑if" videos
  (6–15 min) — the 2016–2018 ones that hit 33M–50M. Evergreen, cheap, simple scripts.
  → [`docs/09-phase1-old-format.md`](docs/09-phase1-old-format.md) +
  [`docs/10-script-writing-simple.md`](docs/10-script-writing-simple.md).
- **Phase 2 (once the channel is built):** move to RECENT / current‑event geopolitics
  (what's happening in the last ~100 days) + the long map‑essay format.
  → `docs/01`–`docs/08`.

## How to start (first week — Phase 1)

1. Read [`docs/09`](docs/09-phase1-old-format.md) (pick a topic from the old‑outlier
   chart) and [`docs/10`](docs/10-script-writing-simple.md) (how to write the script).
2. Pick ONE simple question (e.g. a fresh angle on "how deep is the ocean").
3. Collect 10–20 fact "rungs", smallest → most extreme, each with a source.
4. Write the script with [`templates/script-template-ladder.md`](templates/script-template-ladder.md)
   (or `prompts/03-script-writer.md` told to use the ladder structure). Fact‑check every number.
5. Build the package: title (`docs/02` Phase‑1 formulas) + thumbnail (`docs/04`) +
   description (`templates/description-template.md`).
6. Edit using the `docs/05` style spec. Publish. Log results in a video brief. Repeat.

> Phase‑2 weekly routine (NexLev mining, current events) lives in `docs/06`–`docs/08`.

> This repo is documentation + prompts, not running code. It is designed so a 1–3
> person team (or you + AI + an editor) can ship one high‑quality video per week.
