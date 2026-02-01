# From iPhone tap to dashboard: a streak-based fitness tracker in Power BI

<p align="center">
  <a href="../assets/fitness_dashboard/fitness_dashboard_v2.png">
    <img src="../assets/fitness_dashboard/fitness_dashboard_v2.png" alt="Fitness dashboard" style="width:980px; max-width:100%; height:auto;">
  </a>
</p>

January 2026 flew by and moving cities knocked my routine around more than I expected. But, if it’s not moving cities, it’s work, social plans, or life in general. The excuse changes, the outcome is the same. This year I’d like to make sure I consistently show up.

So I borrowed a trick from something that _does_ keep me consistent: Duolingo. Duolingo users will do almost anything to protect a streak. I wanted that same “don’t break the chain” motivation for fitness.

<p align="center">
  <a href="../assets/fitness_dashboard/Duolingo_Sharing.PNG">
    <img src="../assets/fitness_dashboard/Duolingo_Sharing.PNG" alt="Duolingo streak inspiration" width="320">
  </a>
</p>
<p align="center"><small><em>Inspiration: Duolingo’s streak mechanic for consistency.</em></small></p>

The goal is simple: do something every day while prioritising cardio, strength, and climbing.
The streak continues with a qualifying run (≥ 5 km), climb, or lift, and deliberately includes “Other” activities (e.g. tennis) to keep the system sustainable.

The question was: *can I build a streak I actually want to maintain, using a lightweight data pipeline and a dashboard I’ll check daily?*

---

## Setting
My fitness data was scattered:
- running lived in Strava/Garmin  
- strength sessions lived in iPhone notes  
- climbing lived… mostly in memory  

That made it hard to track progress in one place, especially around the  metric I care about above all else: consistency.

I wanted four things:
- **A streak tracker:** move every day, with most days prioritising lifting, climbing, or running
- **Yearly targets for lifting**, so weights sessions stay engaging and I don’t keep the streak alive purely through other activities
- **Low logging friction**, so the system is simple enough to use daily
- **A framework that rewards consistency over intensity**

For the weights piece, I set **rep-count targets** for squats, deadlifts, bench press, and pull-ups — not tied to hitting heavier numbers, but tied to simply showing up. The targets are rough by design (think: ~100 lifting days × ~30 reps per lift).

---

## Action

### 1) Minimal Google Form pinned on iPhone home screen (fast logging)
<p align="center">
  <a href="../assets/fitness_dashboard/iphoneButton.jpg">
    <img src="../assets/fitness_dashboard/iphoneButton.jpg" alt="iPhone shortcut" height="240">
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="../assets/fitness_dashboard/google_form_v2.jpg">
    <img src="../assets/fitness_dashboard/google_form_v2.jpg" alt="Google Form" height="240">
  </a>
</p>
<p align="center"><small><em>Quick-entry logging: one tap from the home screen → date + activity (plus lightweight fields).</em></small></p>

### 2) Responses land in Google Sheets
<p align="center">
  <a href="../assets/fitness_dashboard/google_sheet.png">
    <img src="../assets/fitness_dashboard/google_sheet.png" alt="Google Sheets responses" style="width:760px; max-width:100%; height:auto;">
  </a>
</p>
<p align="center"><small><em>Form responses captured in Google Sheets (simple “data store” for Power BI to ingest).</em></small></p>

### 3) Dashboard: Power BI ingests the sheet to update the model and visuals
<p align="center">
  <a href="../assets/fitness_dashboard/fitness_dashboard_v2.png">
    <img src="../assets/fitness_dashboard/fitness_dashboard_v2.png" alt="Fitness dashboard" style="width:980px; max-width:100%; height:auto;">
  </a>
</p>
<p align="center"><small><em>Streak tracking, 2026 sessions, best run (≥ 5 km), and progress-to-goal tiles.</em></small></p>

I deliberately avoided ingesting Strava/Garmin data to keep the approach lightweight and low-maintenance.

---

## Outcome
It’s simple enough that I actually want to use it daily, and that’s the whole point. January wasn’t the consistent start I wanted (moving cities), which is exactly why the streak mechanic helps.

**Next target:** build toward a 365-day streak.

Wish me luck.
