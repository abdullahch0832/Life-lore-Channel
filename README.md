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

## How to start (first week)

1. Read `docs/01` and `docs/02` fully.
2. Open `docs/08` and run the NexLev "weekly mining" routine → fill a 20‑idea backlog.
3. Pick 1 idea that matches a proven title formula (`docs/02`) **and** has fresh
   competitor outliers (`docs/06`).
4. Generate the script with `prompts/03-script-writer.md` → edit for accuracy.
5. Build package: thumbnail (`docs/04`) + description (`templates/description-template.md`).
6. Edit using the `docs/05` style spec. Publish. Log results. Repeat.

> This repo is documentation + prompts, not running code. It is designed so a 1–3
> person team (or you + AI + an editor) can ship one high‑quality video per week.
