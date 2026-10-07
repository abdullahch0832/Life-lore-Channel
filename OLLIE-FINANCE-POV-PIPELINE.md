# POV Finance — Complete Video Pipeline (reverse‑engineered from @Olliee_Finance)

> **Yeh kya hai?** Ek single, self‑contained "factory" file. Isko kahin bhi (Notion,
> ChatGPT, Claude, Google Doc) utha kar paste karo aur top se neeche follow karte jao —
> har video isi pipeline se banegi. Analyze kiya gaya competitor: **Ollie Finance**
> (`@Olliee_Finance`) + poora POV‑finance ecosystem, NexLev data se (captured **2026‑10‑07**).
>
> **Scope note:** Aapne kaha tha **data + voice analyze NAHI karni** — isliye voice/VO
> cloning is file mein nahi hai. **Editing style analyze ki gayi hai** (actual video
> dekh kar). Title, script, thumbnail, description, idea‑sourcing aur automation — sab hai.

---

## 0. TL;DR — 60 second mental model

Ollie Finance koi "finance teacher" channel **nahi** hai. Yeh ek **emotional POV
storytelling machine** hai jo *faceless + AI‑assisted animation* use karti hai. Formula:

```
RELATABLE WEALTH FANTASY   →   "POV: You ..." TITLE + MOODY THUMB   →   14–21 min
(secret millionaire,            (2nd person, "nobody knows",            cinematic 2nd‑person
 quiet second income,            "everything changed")                  story over animated
 escaping 9‑to‑5, old money)                                            character + captions
```

3 cheezein jeetni hain, baaki sab noise hai:
1. **Package** = Title + Thumbnail (POV + secrecy + big number).
2. **Emotional arc** = ek "you" jiski zindagi chupke se badalti hai, phir cost/loneliness, phir payoff.
3. **Consistent look** = moody animated character, fast 2–4s cuts, bold yellow captions.

Jo channel yeh 3 cheezein repeat karta hai, woh 1 mahine mein 0 se 170K views per video tak jaata hai (proof neeche).

---

## 1. Competitor snapshot — Ollie Finance (the template)

| Metric | Value |
|---|---|
| Handle | `@Olliee_Finance` |
| Channel ID | `UCFGLwmoU1SuT6t_m3gRERpQ` |
| Joined | **14 May 2026** (yaani naya channel) |
| Subscribers | ~5.09K |
| Videos | 11 |
| Total views | ~634,940 |
| **Avg views/video** | **~57,700** (NexLev) |
| Faceless | **Yes — 98% confidence** |
| AI content | **Yes** (NexLev flag `isAiContent: true`) |
| Format | 2nd‑person "stories", personal finance |
| Country / Lang | United States / English |
| Video length | **14–21 min** (long‑form) |

**Takeaway:** 5 mahine purana, 11 video, aur phir bhi 170K‑view hits. Matlab niche
template itna strong hai ke naya channel bhi tezi se chal sakta hai — **packaging > seniority**.

### 1.1 Ollie ke videos — outlier chart (channel avg ≈ 57.7K)

| Video | Views | Channel outlier | Niche outlier* | Len | Script words |
|---|---|---|---|---|---|
| POV: Your Life After Winning the $600 Million Lottery and You Don't Tell anyone | **170K** | 2.9x | **10.0x** | 14:22 | 2,292 |
| POV: You Quietly Built a Second Income and Told No One | **156K** | 2.7x | **9.1x** | 19:08 | 3,043 |
| POV: You Quietly Built a Portfolio That Pays More Than Your 9‑to‑5 | **132K** | 2.3x | **7.5x** | 21:19 | 3,498 |
| POV: You Silently Building a Holding Company From $0 to $600M, No Body Knows | **111K** | 1.9x | **6.5x** | 14:26 | 2,203 |
| POV: You Quietly Escaped the Rat Race. No One Noticed. | 34K | — | — | 17:08 | — |
| POV: You Building Wealth in Silence, Nobody Knows | 17K | — | — | 12:24 | — |
| POV: Everyone Thinks You're Struggling — You're Actually 7 Figures In and Silent | 15K | — | — | 19:47 | — |
| POV: You Stopped Trying to Look Rich and Your Net Worth Quietly Overtook Everyone's | 10K | — | — | 23:50 | — |
| POV: You Started Thinking Like Old Money and Everything Changed | 4.9K | — | — | 13:51 | — |
| Your Life at Every Stage of Secretly Leaving the 9 to 5 | 3K | — | — | 12:00 | — |
| POV: You Track Every Dollar for 30 Days and Regret Looking | 2K | — | — | 18:08 | — |

\*Niche outlier = views ÷ niche avg (NexLev faceless_outliers). Ye batata hai video niche ke
baaki content se kitni outperform hui.

**Pattern jo saaf nazar aata hai:**
- Jin titles mein **ek specific bada number** + **secrecy** dono hain ("$600 Million" + "Don't Tell anyone") → sabse badi hits.
- Pure abstract/mindset titles ("Old Money thinking", "Track Every Dollar") → sabse kam. **Lesson: concrete fantasy > abstract advice.**
- Video length 12–24 min — longer OK hai (watch‑time niche hai), lekin **hook pehle 15 sec** mein hona zaroori hai.

---

## 2. The mineable ecosystem — "titles/ideas kahan se scrape karni hain"

Yeh woh sibling channels hain jo **bilkul same POV‑finance template** chala rahe hain.
In sabki outlier videos aapki **idea + title swipe file** hain. (NexLev se nikaale, 2026‑10‑07.)

| Channel | Handle | Subs | Videos | Kyun mine karna |
|---|---|---|---|---|
| **POV Finance** | `@POVFinanceUS` | 20.5K | 147 | Template leader — 147 videos ka swipe file, outliers 7–12x |
| **Money Life POV** | `@MoneyLifePOV` | 9.36K | 36 | High views (200K+), 3–5x outliers, clean POV titles |
| **Bille Finance** | `@Bille_Finance` | 26K | 71 | "Your Life at Every Level of Financial Power" (205K) |
| **Will & Wisdom** | `@TheWillWisdom` | 20K | 48 | "Japanese Art of Becoming Rich on a Low Salary" → **877K (30x)** |
| **Lucas Grant** | `@LucasGrant-usa` | 16.1K | 112 | "Living Rich in Secret" → **708K (33x)** |
| **Finance POV** | `@thefinance_pov` | 10.8K | 56 | "Silent Millionaire $650M Nobody Knows" (186K) |
| **Highfinance_View** | `@Highfinance_View` | 11.7K | 75 | "$650 Million Silent Millionaire" → 297K (20x) |
| **Carl Invests** | `@carlinvestsUS` | 5.18K | 89 | "9 Signs Someone is Secretly Wealthy" (126K) |
| **Quiet Capital** | `@QuietCapitalUSA` | 1.85K | 19 | Chhota but 8x outliers — fresh angles |
| **Quiet Compound** | `@QuietCompound-c4z` | 1.47K | 22 | "Built Wealth in Your 30s → 40s" (103K, 11x) |
| **Detrás del Dinero** | `@ElOtroLadoReal` | 1.13K | 43 | **Spanish version** of same template (375K, 28x) → language‑expansion proof |

> **Yeh ek "niche cluster" hai.** Aapka kaam inventing nahi — yeh hai: **in channels ki
> top outliers ko systematically scrape karo → pattern dekho → apna better version banao.**
> Exact tools Section 7 mein.

**Adjacent sub‑themes jo is cluster mein viral hue** (title ke liye raw material):
- Silent / secret millionaire ($650M nobody knows)
- Quiet second income / side hustle in secret
- Escaping the rat race / quitting 9‑to‑5 silently
- "Old money" mindset vs looking rich
- Living rich in secret / stealth wealth
- "Every level/stage of wealth" ladder videos
- Signs someone is secretly wealthy
- Portfolio that out‑earns your salary

---

## 3. TITLE ENGINE — exact formula + swipe

### 3.1 The master formula

```
POV: You [QUIETLY] [past‑tense wealth action] [— and NOBODY knew / everything changed]
```

3 ingredients har winning title mein:
1. **"POV: You ..."** → 2nd person, reader khud ko story mein daalta hai.
2. **Secrecy/quiet word** → *quietly, silently, in silence, no one noticed, nobody knows, told no one*.
3. **A concrete payoff** → bada number ($600M), ya ek status jump (second income, portfolio > 9‑to‑5, holding company).

### 3.2 Title patterns (copy‑paste templates)

- `POV: You Quietly Built [a Second Income / a Portfolio / a Holding Company] and Told No One`
- `POV: Your Life After [winning $X / selling your company] and You Don't Tell Anyone`
- `POV: You Silently Built [asset] From $0 to $[big number], Nobody Knows`
- `POV: You Stopped Trying to Look Rich and [outcome] Quietly Overtook Everyone's`
- `POV: Everyone Thinks You're Struggling — You're Actually [7 Figures In] and Silent`
- `POV: You Started Thinking Like Old Money and Everything Changed`
- `POV: You Escaped the Rat Race. No One Noticed.`
- `[Number] Signs Someone is Secretly Wealthy`
- `Your Life at Every [Stage / Level] of [Financial Power / Leaving the 9‑to‑5]`
- `The [Nationality] Art of Becoming Rich on a Low Salary` (Will & Wisdom = 877K)

### 3.3 Title rules (data‑backed)

- ✅ **Ek specific bada number daalo** jahan possible ho ($600M, $650M, 7 figures) — top hits sab mein number tha.
- ✅ **Secrecy = non‑negotiable.** "Nobody knows / told no one / in silence" har top title mein.
- ✅ **"You" / "Your Life"** rakho — abstract concept titles under‑perform karte hain.
- ✅ Length ~8–14 words. Front‑load the hook.
- ❌ Pure advice/listicle framing ("How to budget", "Track every dollar") → niche mein mar jaata hai.
- ❌ Clickbait jhooth mat — payoff video mein deliver hona chahiye warna watch‑time girega.

> **AI prompt** (Section 8.B) seedha 30 titles generate kar deta hai in rules par.

---

## 4. SCRIPT SYSTEM — the 7‑beat skeleton (4 top scripts se nikala)

Ollie ke char sabse badi videos (lottery, second income, portfolio, holding co.) **bilkul
same skeleton** follow karti hain. Length: **2,200–3,500 words = 14–21 min**. Tense:
**present tense, 2nd person "you"** throughout. Tone: cinematic, intimate, slightly ominous.

### 4.1 The skeleton

| # | Beat | Length | Kaam | Example (lottery video) |
|---|---|---|---|---|
| 1 | **Cold‑open scene (HOOK)** | 0:00–0:30 | Ek mundane, sensory moment + sudden tension. Koi setup nahi, seedha scene. | "You're standing in a gas station at 11:47 at night and your card just got declined for a $4 coffee." |
| 2 | **Inciting discovery** | ~0:30–2:00 | Zindagi badalne waali ghatna + **the secret decision**. | Ticket jeet jaata hai → "You don't tell anyone." |
| 3 | **The thesis / rule** | 1 line | Decision ko ek "rule of the rest of your life" bana do. | "That decision is the first rule of the rest of your life." |
| 4 | **Chronological escalation** | bulk (60–70%) | Time‑stamped beats mein journey: *"The first week… / Three weeks in… / 6 months in… / A year passes… / 18 months in…"* Har stage pe ek naya move + naya emotional layer. | Money slowly move karna, job chhodna, family ko anonymously help karna |
| 5 | **The cost / near‑miss twist** | ~1–2 min | Emotional price: loneliness, ek character jo secret pakad‑ne lagta hai (tension). | "Dana" bar mein shak karti hai → 3 hafte panic |
| 6 | **Philosophical payoff** | ~30–60s | Theme ko universal truth mein resolve karo. | "Money like this isn't freedom. It's a cage with very soft walls." |
| 7 | **CTA + engagement question** | last 20–30s | Like/subscribe + ek open‑ended question comments ke liye. | "If you had $300M… would you finally tell them? Let me know in the comments." |

### 4.2 Micro‑style rules (jo har script mein milay)

- **Sentence rhythm:** chhote punchy sentences + repetition. "You do X. You do Y. You don't tell anyone." Yeh hypnotic rhythm banata hai.
- **2nd person present:** "You walk out…", "You start noticing…" — kabhi "he/she" nahi.
- **Specific numbers everywhere:** "$314 million after the cut", "$40,000 a day", "94 emails, 89 silences, 4 rejections, 1 reply." Specificity = believability.
- **Time‑stamped progression:** "The first week / Month three / By month 12 / 18 months in / A year passes." Yeh backbone hai.
- **Named mini‑character** for conflict (Dana, the brother, a coworker) — ek chhota tension/twist.
- **Sensory grounding:** "the smell of dumpsters and diesel", "fluorescent light", "cold floorboards." Scene ko feel karao.
- **End on a question**, statement pe nahi — comments boost karne ke liye.

### 4.3 Ready hook templates (beat 1)

- "You're standing in [mundane place] at [specific time] and [small humiliating/ordinary thing] just happened."
- "The alarm hits at 5:45 a.m. It isn't a harsh sound anymore…"
- "It's 7:41 on a Tuesday morning and you're [doing boring routine thing]."
- "You're [age] years old, sitting in [boring workplace], [doing pointless task]. Nobody sees you. That's the moment it happens."

> Full script generate karne ka AI prompt Section 8.C mein — yeh 7 beats enforce karta hai.

---

## 5. THUMBNAIL SYSTEM

(Thumbnails ka visual pattern video‑frame analysis + niche se nikala; raw image download proxy ne block kiya, lekin style niche‑wide consistent hai.)

**Formula:** `Animated character (back/side view) + ONE moody scene + 2–4 giant words + a big number/money cue`.

- **Character:** consistent faceless/animated protagonist (Ollie: grey hoodie + black cap), aksar **peeth ya side se** — reader khud ko project kar sake.
- **Background:** cinematic, desaturated, dark cool tones (blue/grey), ek strong neon/warm accent (lottery sign yellow, "declined" red, city lights, luxury interior silhouette).
- **Text:** 2–4 bade bold words, **sans‑serif, mostly UPPERCASE**, yellow/white. Examples: `$600,000,000`, `NOBODY KNOWS`, `TOLD NO ONE`, `SILENT MILLIONAIRE`.
- **Mood:** mystery + aspiration. Luxury cheez chupi/silhouette (mansion, car, cash) — flashy nahi, *secret* feel.
- **Consistency:** same character + same text style har video — channel branding ban jaati hai.
- **Rule:** thumbnail title ko *repeat* na kare — title kahta hai "quietly built second income", thumb dikhata hai `$640/DAY` + hoodie wala banda laptop pe. Curiosity gap.

**Mistakes to avoid:** stocky corporate smiley faces, 10 cheezein ek saath, chhota text, bright/happy palette (yeh niche moody hai).

---

## 6. EDITING / VISUAL STYLE (actual video analyze ki gayi)

Ollie ka top video (lottery) dekh kar nikala gaya **replicable** spec:

| Element | Spec |
|---|---|
| **Visual type** | 2D **hand‑drawn / illustrated character animation** (AI‑assisted). **Stock footage nahi.** |
| **Movement** | Mostly static illustrated frames + **Ken Burns** (slow zoom/pan) + chhoti character animations (blink, mouth, haath). |
| **Cut frequency** | **Fast — har 2–4 second** naya shot. Watch‑time ke liye kabhi static nahi rehta. |
| **Color grade** | Moody, cinematic. Desaturated dark cool tones (blue/grey) + vibrant neon accents (red "declined", yellow lottery sign). |
| **Captions** | Bade, bold, centered sans‑serif at bottom. **Yellow with white highlight** on emphasis words. |
| **FX** | Subtle **film grain**, heavy **vignette**, light **bloom/glow** on screens & lights. |
| **Aspect / framing** | 16:9 widescreen. Medium shots of character + close‑ups of key objects (wallet, phone, ticket). |
| **Character** | **Ek consistent recurring protagonist** (same outfit) — narrative ko ground karta hai. |

### 6.1 How to replicate (toolchain options)

1. **Script → scene list:** har 2–4 sec ke liye ek image‑prompt banao (AI se, Section 8.D).
2. **Image generation:** Midjourney / Leonardo / Flux se consistent character (character reference / same seed + same outfit description). Moody cinematic style keywords: *"moody cinematic 2D illustration, desaturated blue‑grey, film grain, vignette, volumetric light, neon accent"*.
3. **Animate:** Ken Burns (CapCut/Premiere keyframe zoom), ya image‑to‑video (Runway/Kling/Hailuo) halki motion ke liye.
4. **VO:** *(aapne voice step abhi skip kaha hai — jab chaho ElevenLabs/PlayHT se karna.)*
5. **Captions:** CapCut auto‑captions → yellow bold style, bottom center, keyword highlight.
6. **Grade + FX:** LUT (moody teal‑orange/cool), film‑grain overlay, vignette, glow. Cuts 2–4s pe tight.
7. **Music:** low ambient/cinematic underscore, subtle — dialogue‑driven, loud nahi.

---

## 7. NEXLEV AUTOMATION PIPELINE — "which tool, when"

Yeh aapka weekly engine hai. Har step ek NexLev tool se map hota hai.

### STEP 1 — Ecosystem lock & refresh (mahine mein ek baar)
- `channel_resolver` → har competitor (Section 2) ka channel ID nikaalo.
- `get_similar_channels` (level 3, async → poll `get_similar_channels_status`) → naye sibling channels dhoondo. Section 2 ki list grow karo.
- `latest_discovered_faceless_niches` → adjacent faceless niches jo abhi ubhar rahe hain.

### STEP 2 — Idea/title mining (har hafte)
- **Main mine:** `faceless_outliers_videos`
  - `query`: `"POV quietly building wealth in silence, secret millionaire, escaping the rat race"`
  - `minOutlierScore: 3`, `languages: ["english"]`, `videoType: "long"`, `isFaceless: true`
  - Jo 3x+ outlier aayein unki **title + outlier + views** ek sheet mein daalo.
- **Per‑competitor scrape:** har channel pe `youtube_channel_outliers` (`min_outlier_threshold: 2`) → unki proven viral titles.
- **Broad title scrape:** `search_videos`
  - `query: "POV: You"`, `minOutlierScore: "2"`, `minView: "100000"`, `sortBy: "outlierScore"`, `englishOnly: true`.
- Sab titles ko ek "swipe file" mein collect karo → `save_to_swipefile` (NexLev) ya apni sheet.

### STEP 3 — Validate the idea (publish se pehle)
- `get_similar_videos` / `search_videos` exact‑match → confirm yeh angle kitni baar / kitna bada hit hua.
- `get_channel_analytics` on the channel that nailed it → consistency check (one‑hit ya repeatable?).
- **(Monetization/RPM — optional)** `get_video_rpm` / `check_channel_monetization` → niche ki kamai samajhne ke liye.

### STEP 4 — Study the winner's structure (clone the skeleton, not the words)
- `get_bulk_video_transcripts` (up to 10) top outliers ke → Section 4 skeleton verify/update.
- `youtube_video_details` → unke **tags + description** scrape karo (apni SEO ke liye).

### STEP 5 — Produce
- Title → Section 3 + AI prompt 8.B.
- Script → Section 4 + AI prompt 8.C.
- Thumbnail → Section 5; `generate_thumbnail` / `get_similar_thumbnails` / `edit_thumbnail` se iterate.
- Edit → Section 6 spec.
- Description/tags → Section 9 template (winner ke tags ko blend karo).

### STEP 6 — Publish & track
- Apni best outliers `save_to_swipefile` → `list_swipefile_folders` se organize.
- 48–72 ghante baad views vs channel‑avg (57K benchmark) compare → jo 2x+ ho woh theme **dubara**, naye angle se.

### 7.1 One‑line tool map

| Chahiye | NexLev tool |
|---|---|
| URL → channel ID | `channel_resolver` |
| Viral POV‑finance video ideas | `faceless_outliers_videos` (semantic query, outlier 3+) |
| Ek competitor ki hit titles | `youtube_channel_outliers` |
| Keyword se broad title scrape | `search_videos` (`query:"POV: You"`, filters) |
| Naye sibling channels | `get_similar_channels` (lvl 3) + `get_similar_channels_status` |
| Ubhartے faceless niches | `latest_discovered_faceless_niches` |
| Winner ka script skeleton | `get_bulk_video_transcripts` |
| Tags/description chori | `youtube_video_details` |
| Kamai check | `get_video_rpm`, `check_channel_monetization` |
| Thumbnail banao/edit | `generate_thumbnail`, `edit_thumbnail`, `get_similar_thumbnails` |
| Winners save/organize | `save_to_swipefile`, `list_swipefile_folders` |

---

## 8. COPY‑PASTE AI PROMPTS

> In prompts ko ChatGPT/Claude mein paste karo. `{{...}}` bharo.

### 8.A — Idea → 10 angles
```
You are a YouTube strategist for a FACELESS 2nd‑person POV personal‑finance storytelling
channel (style: @Olliee_Finance / "POV: You quietly built wealth, nobody knows").
Theme seed: {{seed e.g. "secret second income"}}.
Give me 10 fresh video ANGLES. Each must be: an emotional wealth fantasy, 2nd person,
with built‑in secrecy, and a concrete payoff (a number or a clear status jump).
For each: (a) one‑line premise, (b) the "cost/twist" that creates emotional tension.
No generic advice topics. Rank by viral potential.
```

### 8.B — 30 titles
```
Act as a YouTube title writer for a POV personal‑finance story channel.
Topic: {{topic}}.
Rules: start with "POV: You" or "Your Life"; include a secrecy word (quietly/silently/
nobody knows/told no one/no one noticed); include ONE concrete payoff (a big specific
number OR a clear status jump); 8–14 words; 2nd person; no false promises.
Give 30 titles, best first. After each, add a 3‑word reason it works.
```

### 8.C — Full script (the 7‑beat skeleton)
```
Write a {{14}}–{{18}} minute YouTube script ({{2600}}–{{3200}} words) for a faceless
2nd‑person POV personal‑finance STORY. Title: "{{title}}".
Voice: present tense, 2nd person ("you"), cinematic, intimate, slightly ominous.
Follow EXACTLY this 7‑beat structure:
1) COLD‑OPEN HOOK (first 2 sentences): drop "you" into a mundane sensory moment at a
   specific time/place, then a sudden small tension. No intro, no "welcome back".
2) INCITING DISCOVERY + the secret decision ("you tell no one").
3) THESIS: turn the decision into "the first rule of the rest of your life".
4) CHRONOLOGICAL ESCALATION (60–70% of script): progress through time‑stamped beats
   ("the first week… / three weeks in… / 6 months in… / a year passes… / 18 months in…").
   Each stage = one new concrete move + one new emotional layer. Use SPECIFIC numbers.
5) THE COST / NEAR‑MISS: introduce ONE named minor character who nearly exposes the
   secret; show loneliness/paranoia as the real price.
6) PHILOSOPHICAL PAYOFF: resolve into a universal truth about money ("real wealth is…").
7) CTA + an open‑ended QUESTION to drive comments.
Style rules: short punchy sentences with rhythmic repetition; sensory grounding; never
third person; never break character to lecture. End on the question, not a statement.
```

### 8.D — Scene/image prompts for the edit
```
Here is my script: {{paste script}}.
Break it into shots of ~3 seconds each. For EACH shot output:
- timestamp range
- one line of the narration it covers
- an image‑gen prompt describing the scene in this exact style:
  "moody cinematic 2D illustration, consistent character = {{grey hoodie, black cap, back/
   side view}}, desaturated blue‑grey palette with one neon accent, film grain, vignette,
   volumetric light, 16:9".
Keep the SAME character description every shot for consistency.
```

---

## 9. DESCRIPTION + TAGS TEMPLATE (SEO)

Ollie ka description pattern (real): 1 hook line → 2–3 para "what this video breaks down"
→ subscribe line → **disclaimer** → hashtags. Copy this:

```
{{One‑line emotional hook restating the premise.}}

In this video, we break down {{what the story explores — financially, psychologically}}.
We explore {{3–4 sub‑ideas: mindset shift, the practical mechanics, the hidden cost}}.

Whether you care about personal finance, wealth psychology, or how money really works,
this gives you a clear, no‑hype breakdown.

Subscribe for more deep dives into finance, wealth, and the quiet decisions that change your life.

⚠️ Disclaimer: This content is for educational and entertainment purposes only and is not
financial advice. Always consult a licensed financial advisor before making decisions.

#PersonalFinance #WealthManagement #FinanceExplained #{{Topic}} #MoneyMatters
```

**Tags** (Ollie actually uses these — blend with the winner‑video tags you scraped in Step 4):
`personal finance, building wealth quietly, silent wealth building, passive income explained,
second income, financial freedom, us finance, usa lifestyle, wealth explained, high net worth
financial planning` + topic‑specific ones.

---

## 10. WEEKLY FACTORY CHECKLIST (ship 1–2 videos/week)

```
[ ] MON  Mine: faceless_outliers_videos (outlier 3+) + 2 competitors' youtube_channel_outliers
[ ] MON  Pick 1 angle (concrete fantasy + secrecy + number). Validate with search_videos.
[ ] TUE  Title: run prompt 8.B → pick 1. Thumbnail concept: 2–4 words + character + number.
[ ] TUE  Script: run prompt 8.C → fact/flow pass → enforce the 7 beats + specific numbers.
[ ] WED  Scene list (8.D) → generate images (consistent character) → build thumbnail.
[ ] THU  Edit: 2–4s cuts, Ken Burns, moody LUT, grain+vignette, yellow bold captions.
[ ] FRI  Description + tags (Section 9). Publish. save_to_swipefile the references.
[ ] +72h Compare views vs 57K avg. 2x+ theme → repeat with a new angle next week.
```

---

## 11. Guardrails (channel safe rakho)

- Finance **story/entertainment** frame rakho; har description mein **"not financial advice" disclaimer** (Ollie bhi karta hai, "Education" category).
- Thumbnail/title ka payoff video mein **deliver** karo — warna retention aur CTR dono girenge.
- Specific numbers plausible rakho (believable range), kyunki yeh fiction‑style POV hai, "guaranteed returns" claim nahi.
- Faceless + AI content YouTube pe allowed hai jab **transformative + original narrative** ho (yeh hai) — doosron ka footage/script copy mat karo; sirf *structure* clone karo, words apne.

---

### Appendix — raw data source
Captured via NexLev MCP, **2026‑10‑07**: `youtube_channel_about`, `check_faceless_channel`
(98% faceless), `youtube_channel_videos`, `youtube_channel_outliers`, `youtube_video_details`
(x2), `get_bulk_video_transcripts` (4 top scripts, fully read), `watch_youtube_video_and_ask`
(visual/editing analysis of the $600M lottery video), `faceless_outliers_videos` (ecosystem +
niche outliers). Channel ID `UCFGLwmoU1SuT6t_m3gRERpQ`.
