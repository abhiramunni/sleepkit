# SleepKit — Sleep Better, Wake Brighter

Sleep runs in 90-minute cycles. Wake in the middle of one and you feel groggy for an hour; wake at the end and you feel human. SleepKit finds your best bedtime, logs your nights, and tells you honestly what your sleep debt is.

Live: **https://abhiramunni.github.io/sleepkit/**

## What it does

- **Tonight card** — Set your bedtime and wake time once. A live countdown ticks to bedtime (or to wake-up while you sleep), with your last-coffee time (8 hours before bed), screens-off time (1 hour before) and wind-down time (30 minutes before) worked out for you.
- **Cycle finder** — Pick when you must wake up and it works backwards in 90-minute cycles (+14 minutes to fall asleep) to find your best bedtime; or pick when you can sleep and it finds the gentlest wake-up. Four, five or six full cycles — never a half cycle.
- **Sleep log** — Log a night in thirty seconds: date, bedtime, wake time, quality (1–5), what shaped it (warm milk, late screen, rain sounds…) and a one-line note. Newest first, tap to delete.
- **The week in sleep** — Average night, best night, sleep debt vs your target, 7-hour nights, and a streak ring of 7-hour nights. A bar chart of the last seven nights against a dashed target line.
- **Power-nap timer** — 10 / 20 / 30-minute presets with a countdown ring and a gentle chime. Twenty minutes is the classic: long enough to sharpen you, short enough to stay out of deep sleep.
- **Wind-down routine** — Six fixed steps in the same order every night, with a progress ring. A fixed routine is a signal to your brain that sleep is coming.
- **Pay it back** — Your sleep debt, and how many nights of going to bed 15 / 20 / 30 minutes earlier clears it.
- **Six plain-language guides** — The 90-minute cycle, caffeine's 5-hour half-life, the 20-minute nap, snoring (when to worry), exam-night sleep, and shift work & jet lag.
- **Your data stays yours** — Everything is saved in localStorage on your device. Nothing is uploaded. Copy a one-paragraph sleep summary, remove the sample nights, or erase everything with two taps.

## The maths (hand-checked)

- Wake 6:30 AM → 5 cycles = bed 10:46 PM (6:30 − 7h 30m − 14 min). 4 cycles = 12:16 AM, 6 cycles = 9:16 PM.
- Bed 11:00 PM → 5 cycles = wake 6:44 AM (11:00 PM + 14 min + 7h 30m). 4 cycles = 5:14 AM, 6 cycles = 8:14 AM.
- Seed week (13–19 Nov 2026): 7 nights, average 6h 59m, best 7h 20m, debt 3h 35m vs the 7h 30m target, 6 of 7 nights at 7 hours or more, 3-night streak.
- Debt payoff: 3h 35m clears in 15 nights at +15 min, 11 nights at +20 min, 8 nights at +30 min.

## Tech

- One single self-contained `index.html` — no backend, no signup, no build step.
- Two AI-generated warm-editorial photos embedded as base64 (bedroom at dusk, bedside flat-lay).
- Fraunces + Inter, warm ember-night palette (deep espresso, amber, gold, terracotta).
- Full-screen cinematic intro (moon, twinkling stars, staggered title, progress, tap-to-skip; quick version on return visits) and a 3-step onboarding tour.
- QA: 93/93 headless jsdom assertions, `node --check` clean, zero uncaught JS errors.

## Privacy note

SleepKit is a planning and tracking tool, not medical advice. If you snore loudly, gasp in your sleep, feel exhausted despite full nights, or have trouble sleeping for more than a few weeks, talk to a doctor.
