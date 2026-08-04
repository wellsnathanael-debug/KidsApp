# ⚽ Goal Getters — Learn & Score (Stadium Night edition)

A gamified educational football app for three young footballers — **Ezra (6)**, **Avery (10)** and **Sols (12)**.
Answer age-appropriate questions to earn penalty kicks in a floodlit stadium, defend the goal,
win the World Cup, duel each other, and unlock trophies, footballs and your own hand-drawn flag.

**The whole app lives in `index.html` with zero dependencies** (the extra files are the
home-screen icons and web-app manifest).

Play it here: **https://wellsnathanael-debug.github.io/KidsApp/**

## Game modes

- **Shootout** — pick your nation and your opponent from **32 countries**, then it's a real
  best-of-5 penalty shootout: answer a question to earn each kick (wrong answer = blazed over!),
  swipe to shoot, then pick where to dive for the opponent's kick. Level after five?
  **Sudden death.** Post and bar included — listen for the ping.
- **World Cup** — three tiers to climb (**Bronze → Silver → Golden**, each unlocked by winning the
  one before). Every cup is a proper tournament: **three group matches with a league table**
  (draws allowed), then a semi-final and the final against **boss keepers** — Iron Hands Ivan never
  dives left, El Pulpo has octopus reach, Robo-Keeper 3000 reads your mind. **Your run is saved**,
  so you can stop mid-tournament and come back to it tomorrow.
- **Skills Arena** — three quick games for five spare minutes: **Crossbar Challenge**,
  **Target Practice** and **Quickfire Maths**. Beat your personal best to win a sticker pack.
- **Duel** — two players, one iPad, pass-and-play. Each child answers questions for **their own age**,
  so a 6-year-old can fairly beat a 12-year-old. 5 kicks each, sudden death if level.
- **Sticker Album** — collect **30 stickers** across four sets (Nations, Mascots, Skills and rare
  foil Goldens). Packs are earned by winning matches, completing daily challenges and finishing
  drawings, and open one card at a time. Got a spare? **Give it to a brother or sister.**
- **Drawing Studio** — four ghost-guided tutorials (Team Badge, Football, Lion Mascot, and
  **Design Your Flag** — your finished flag flies on the match scoreboard). Each finished tutorial
  earns a ⭐ Super Shot (freezes the keeper) in every match.
- **Trophy Cabinet & Kit Locker** — 19 achievements, cup wins per tier, 5 unlockable footballs and
  6 **goal celebrations** (knee slide, backflip, robot dance, shirt over head, heart hands).

## Coming back tomorrow

- **Daily Challenge** — a new challenge every day ("score 5 goals", "make 3 saves", "win a shootout"),
  the *same one for all three children* so they can compete. Completing it earns a sticker pack and
  builds a **streak** — with bonus packs at 3, 7 and 14 days.
- **Saved World Cup runs** — an unfinished semi-final is waiting when they next open the app.
- **The album's empty slots** — the most reliable "just one more game" there is.

## Learning content (UK curriculum-flavoured, UK English throughout)

| Player | Maths | Other |
|--------|-------|-------|
| Ezra (6)  | Addition & subtraction under 20, counting pictures | Word-to-picture matching |
| Avery (10)| Times tables, fractions of amounts, word problems starring the three of them | UK geography & basic science |
| Sols (12) | BODMAS, simple algebra, percentages (timed!) | General knowledge |

The robot keeper also gets sharper the longer your scoring streak — hat-tricks must be earned.

## Running it

- Visit the link above, or open `index.html` directly — no internet needed after that.
- On iPad: open in Safari → **Share → Add to Home Screen** for a full-screen app with its own icon.
- Progress (high scores, trophies, unlocks, flags) saves per player in the browser's local storage.

## Tech notes

- Single-file HTML5 + CSS3 + ES6 JavaScript; canvas-rendered stadium (night sky, floodlights,
  animated crowd, adboards, rippling net) and a layered drawing canvas.
- Pointer Events (with coalesced events) for smooth finger, Apple Pencil and mouse input;
  arrow keys work for diving on a keyboard.
- All sound is synthesised WebAudio — crowd ambience, cheers, whistles, woodwork pings — no audio files.
- System font stack (renders SF Pro on Apple devices) and hand-rolled CSS, so it works completely offline.
- Emoji flags render natively on Apple devices; on Windows they may appear as letter codes.
