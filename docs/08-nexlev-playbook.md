# 08 — NexLev Playbook (which tool, when, exactly)

You asked to be guided **using NexLev**. This is the operating manual: the exact NexLev
tools to run for each job, in order. Tool names are the NexLev MCP tools
(`mcp__NexLev__*`). Everything below was used to build this very system, so it's proven.

## Core concepts (keep in mind)
- **Outlier score** = video views ÷ channel average. ≥2 strong, ≥3 exceptional.
- **Semantic search** (`search_niche_finder_channels`, `faceless_outliers_videos`): a
  natural‑language `query` matches by *meaning*. Use `query:"*"` for pure numeric filtering.
  On a semantic query, **don't set `sortBy`** (it discards relevance).

---

## Routine A — Analyze a competitor (one‑time per channel)
Run this on RealLifeLore and on every peer in `docs/06`.

1. `channel_resolver` → paste the channel URL, get the `channelId`.
   - RealLifeLore = `UCP5tjEmvPItGyLhmjdwP7Ww`.
2. `youtube_channel_about` → subs, total views, video count, keywords, join date.
3. `get_channel_analytics` → growth + engagement overview.
4. `youtube_channel_outliers` (set `min_outlier_threshold: 1.8`, `max_videos: 200`) →
   their biggest *relative* hits = the templates worth cloning.
5. `youtube_channel_videos` (`sort_by: popular`) → all‑time winners for packaging study.
6. (Optional) `get_similar_channels` (level 3, async → poll `get_similar_channels_status`)
   → map the competitive cluster. *Note: it returns a broad set incl. news channels;
   filter to true map‑essay peers yourself.*

## Routine B — Weekly idea + outlier mining ⭐ (do every week)
This fills your backlog (`docs/06` Well 4).

1. `faceless_outliers_videos` with a semantic `query` describing the niche, e.g.
   *"geography geopolitics explainer, why a country is empty, how geography shaped a
   nation, map documentary"*, plus filters:
   - `videoType: "long"`, `minOutlierScore: 3`, `isFaceless: true`, `limit: 25`.
   - Leave `sortBy` unset. Read the returned `videoTitle`, `outlierScore`, `channelSubCount`.
2. For each promising hit, note: title → which `docs/02` formula → the paradox/emotion.
3. `get_similar_videos` (pass a winning `videoId` or title) → find adjacent angles / the
   content gap you can fill.
4. `search_niche_finder_channels` (semantic query, same theme) with filters like
   `isFaceless:true`, `maxSubscribers: 3000000`, `minAvgVideoLength: 600` → discover new
   peer channels to add to your tracking list, and spot *growing* niches (clusters of
   `outlierScore ≥ 2`, recent `createdAt`).
5. Add 15–20 rows to the backlog.

## Routine C — Validate ONE idea before you commit
Before scripting, confirm demand.

1. `search_videos` / `youtube_search` for your exact topic → does the angle already have
   big views? Is there a packaging gap you can beat?
2. `get_similar_videos` on the closest existing hit → confirm the demand + find your twist.
3. (If you want the earning case) `get_video_rpm` on a comparable video, and
   `check_video_monetization` → sanity‑check the money side of the topic/geo.

## Routine D — Study a specific winning video (script + edit learning)
1. `youtube_video_details` → length, description (**reveals their tools/credits!**), tags.
2. `get_video_transcript` (or `get_bulk_video_transcripts`) → study the 8‑beat arc,
   hooks, analogies, sponsor bridge (`docs/03`). *This is cheap — always prefer it.*
3. `youtube_video_comments` → what the audience loved / asked / corrected = your angle +
   accuracy checklist.
4. **Only if you need the visuals** → `watch_youtube_video_and_ask` (expensive; use
   `startOffset`/`endOffset` to clip). Ask it to break down the editing style for the
   `docs/05` checklist. *(This is exactly how `docs/05` was built.)*

## Routine E — Thumbnail research & drafts
1. `get_similar_thumbnails` → what already ranks for your topic; find the visual gap.
2. `generate_thumbnail` → AI draft from a prompt (use the `docs/04` layout recipe).
3. `edit_thumbnail` → iterate; poll `get_thumbnail_edit_status` / `get_thumbnail_generation_status`.
4. `save_to_swipefile` / swipefile tools → keep a library of thumbnails that work.

## Routine F — Track YOUR channel once it's live (optimize)
If you connect your channel to NexLev (`list_my_youtube_channels`):
- `get_my_channel_overview`, `get_my_top_videos` → what's working.
- `get_my_audience_retention` → where viewers drop (fix those script beats in `docs/03`).
- `get_my_traffic_sources` → confirm browse/suggested is the engine (it should be).
- `get_my_revenue_report` / `get_geography_revenue` / `get_video_rpm` → the money view.
- `get_short_vs_long_views` → whether to invest in Shorts as a funnel.

## Niche health check (optional, quarterly)
- `get_niche_overview` (+ `get_niche_overview_status`) on "geography/geopolitics
  explainer" → competitive landscape, saturation, RPM.
- `latest_discovered_faceless_niches` → spot emerging adjacent niches early.

---

### Quick reference: job → tool

| I want to… | NexLev tool |
|---|---|
| URL → channelId | `channel_resolver` |
| Competitor stats | `youtube_channel_about`, `get_channel_analytics` |
| Their biggest relative hits | `youtube_channel_outliers` |
| Mine viral ideas in the niche | `faceless_outliers_videos` (semantic) |
| Discover peer channels | `search_niche_finder_channels` (semantic) |
| Adjacent angles to a hit | `get_similar_videos` |
| A video's script | `get_video_transcript` |
| A video's tools/metadata | `youtube_video_details` |
| A video's edit/visuals | `watch_youtube_video_and_ask` (last resort) |
| Audience reaction | `youtube_video_comments` |
| Thumbnail ideas | `get_similar_thumbnails`, `generate_thumbnail` |
| My own channel analytics | `get_my_*` family |
