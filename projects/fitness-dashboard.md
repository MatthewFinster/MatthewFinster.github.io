# Fitness streak dashboard (Power BI)

## Problem
My fitness data was scattered across apps and iPhone notes, so it was hard to track progress towards goals in one place.
I wanted a simple system to log activities daily (run ≥ 5 km, climb, or weights) and keep consistency using a streak mechanic (Duolingo-style).

## Action
- Minimal Google Form pinned on iPhone home screen (fast logging)
- Responses land in Google Sheets
- Power BI ingests the sheet to update the model and visuals
- Deliberately avoided Strava/Garmin ingestion to keep it lightweight

## Dashboard


## What I built
- Current streak + last 7 days strip (C / R / W)
- Best run table filtered to runs ≥ 5 km
- Progress-to-goal KPI tiles (e.g., 342 / 3000) with small progress bars

## Outcome
It’s lightweight enough that I actually use it daily. January wasn’t as consistent as I wanted (moving cities), which is exactly why the streak mechanic helps. Next target: build toward a 365-day streak.
