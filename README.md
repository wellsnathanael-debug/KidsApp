# ⚽ Goal Getters! — Learn & Score

A gamified educational web app for three young footballers — **Ezra (6)**, **Avery (10)** and **Sols (12)**.
Answer questions to earn penalty kicks, defend the goal when you slip up, follow
step-by-step drawing tutorials, and unlock trophies and custom footballs along the way.

**The whole app lives in `index.html` with zero dependencies** (the extra files are just the
home-screen icons and web-app manifest).

Play it here: **https://wellsnathanael-debug.github.io/KidsApp/**

## Running it

- **Simplest:** double-click `index.html` (or open it in Safari/Chrome). That's it.
- **iPad:** host the file anywhere (or AirDrop it and open in Safari), then *Share → Add to Home Screen* for a full-screen app feel.
- **Local server (optional):** `python3 -m http.server` in this folder, then visit `http://localhost:8000`.

Progress (high scores, trophies, unlocks) is saved per player in the browser's local storage.

## How it works

1. **Pick your player** — Ezra 🦁 (6), Avery 🦊 (10) or Sols 🐺 (12). Each profile has its
   own questions, difficulty, saved progress and trophies.
2. **Penalty Shootout** — 5 rounds against the Rival Robots:
   - Answer a question correctly → **you take a penalty**. Swipe (finger/stylus) or drag
     (mouse) from the ball to aim; a longer swipe means more power. Corners beat the keeper!
   - Answer wrongly → **the Robots shoot** and you pick where to dive (tap the buttons or
     use the arrow keys on a keyboard).
   - Goals score 10 points (streak bonuses stack), saves score 5.
3. **Drawing Studio** — three step-by-step tutorials (Team Badge 🛡️, Classic Football ⚽,
   Lion Mascot 🦁) with dotted ghost guides, a colour palette, brush sizes, eraser and undo.
   Finishing a tutorial unlocks a special football **and** earns a ⭐ Super Shot
   (freezes the robot keeper) in every shootout.
4. **Trophy Cabinet & Kit Locker** — collect 10 achievements, choose your football
   (Classic, Golden, Rainbow, Fireball) and your goalkeeper kit colour.

## Learning content (UK curriculum-flavoured, UK English throughout)

| Player | Maths | Other |
|--------|-------|-------|
| Ezra (6)  | Addition & subtraction under 20, counting pictures | Word-to-picture matching |
| Avery (10)| Times tables, fractions of amounts, word problems starring the three of them | UK geography & basic science |
| Sols (12) | BODMAS, simple algebra, percentages (timed!) | General knowledge |

Age 6 gets bigger buttons, simpler wording and no timer; ages 10 and 12 race a gentle
countdown for extra challenge.

## Tech notes

- Single-file HTML5 + CSS3 + ES6 JavaScript; two `<canvas>` games (shootout + drawing).
- Pointer Events (with coalesced events) for smooth finger, Apple Pencil and mouse input.
- WebAudio synth sound effects (mutable) — no audio files.
- Hand-rolled CSS rather than a CDN framework so the app works completely offline.
