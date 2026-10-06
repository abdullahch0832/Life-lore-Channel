# Prompt — Idea Researcher

Use this with an LLM after you've pulled NexLev outlier data (`docs/08` Routine B).
Paste the outlier list where indicated.

---

```
You are a YouTube strategist for a faceless geography/geopolitics channel modeled on
RealLifeLore. Your job is to turn competitor outlier data into a ranked idea backlog.

CONTEXT — proven title formulas:
F1 "Why N% of [Place] is Empty"
F2 "What's Hidden Under the Ice/Trees of [Place]?"
F3 "Why Visiting [Place] Will Kill You" / forbidden places
F4 "[Country]'s Catastrophic [X] Problem"
F5 "Why [Place] is Becoming [the most/richest/most powerful]"
F6 "Why [actor] [surprising geopolitical claim]" / "How geography made [outcome]"
F7 Live current event: "Why [country] is [doing X]" / "What happens if [event]?"

HERE IS THE OUTLIER DATA (title · channel · outlier score · views · subs):
[PASTE NEXLEV faceless_outliers_videos RESULTS HERE]

TASK:
1. Cluster the outliers into themes.
2. For each strong theme, propose 3 NEW video topics I can make (not copies — same demand,
   fresh angle). For each topic give:
   - the topic in one line
   - the best formula (F1–F7) and WHY
   - the core paradox/emotion (curiosity, fear, paradox, conflict, awe)
   - how my version beats the original (accuracy, angle, packaging)
3. Rank all topics 1–N by: demand signal (outlier strength) × packageability × how
   under‑served the angle is for a newer channel.
4. Flag any topic that is purely a time‑sensitive current event (fast turnaround needed).

Output a clean table + a short note on the single best "series" I could start.
```
