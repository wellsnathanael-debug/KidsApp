# ⚽ Goal Getters — Learn & Score (Stadium Night edition)

A gamified educational football app for three young footballers — **Ezra (6)**, **Avery (10)** and **Sols (12)**.
Answer age-appropriate questions to earn penalty kicks in a floodlit stadium, defend the goal,
win the World Cup, duel each other, and unlock trophies, footballs and your own hand-drawn flag.

**The whole app lives in `index.html` with zero dependencies** (the extra files are the
home-screen icons and web-app manifest).

Play it here: **https://wellsnathanael-debug.github.io/KidsApp/**

## Game modes

- **Match Day** — a full football match, where **every question is a phase of play**. Answer
  correctly and your team completes a pass and moves up the pitch; get it wrong and you're tackled.
  Reach the final third for a real shot (swipe), and dive to keep them out when they break through.
  Top-down pitch view, a running match clock, **live commentary**, and full-time stats for
  possession, shots and passes. Choose a **Quick Match** (one half) or a **Full Match** (two halves
  with half-time) at kick-off — it defaults sensibly to your skill rank.
- **Season** — a five-match league against five clubs, with a proper table. Played as Match Day
  fixtures, saved between sessions, and finishing top makes you champions.
- **Shootout** — pick your nation and your opponent from **32 countries**, then it's a real
  best-of-5 penalty shootout: answer a question to earn each kick (wrong answer = blazed over!),
  swipe to shoot, then pick where to dive for the opponent's kick. Level after five?
  **Sudden death.** Post and bar included — listen for the ping.
- **World Cup** — five tiers to climb (**Bronze → Silver → Golden → Platinum → Legends**, each
  unlocked by winning the one before), and the field grows as you go: 8 nations at Bronze/Silver,
  16 with a quarter-final at Golden/Platinum, and **all 32 nations with a round of 16** in the
  Legends Cup. Every cup starts with **three group matches and a league table** (draws allowed),
  then knockouts against **12 named boss keepers** — Iron Hands Ivan never dives left, Bouncer Bruno
  laughs off power shots, Corner Cat owns the corners. Each taunt hints at how to beat them, and no
  keeper repeats within a tournament. **Your run is saved**, so you can stop mid-tournament
  and come back to it tomorrow. Winning Legends unlocks the Galaxy Ball.
- **Skills Arena** — three quick games for five spare minutes: **Crossbar Challenge**,
  **Target Practice** and **Quickfire Maths**. Beat your personal best to win a sticker pack.
- **Duel** — two players, one iPad, pass-and-play. Each child answers questions for **their own age**,
  so a 6-year-old can fairly beat a 12-year-old. 5 kicks each, sudden death if level.
- **Sticker Album** — collect **60 stickers** across six sets (Nations, Mascots, Stadiums, Skills,
  Legends and rare foil Goldens) — and every sticker also has a rare **shiny** version, so even a
  finished album leaves something to chase. Packs are earned by winning matches, completing daily
  challenges and finishing drawings, and open one card at a time. Got a spare? **Give it to a
  brother or sister.**
- **Drawing Studio** — four ghost-guided tutorials (Team Badge, Football, Lion Mascot, and
  **Design Your Flag** — your finished flag flies on the match scoreboard). Each finished tutorial
  earns a ⭐ Super Shot (freezes the keeper) in every match.
- **Trophy Cabinet & Kit Locker** — 29 achievements, cup wins per tier, 6 unlockable footballs and
  6 **goal celebrations** (knee slide, backflip, robot dance, shirt over head, heart hands).

## Coming back tomorrow

- **Daily Challenge** — a new challenge every day ("score 5 goals", "make 3 saves", "win a shootout"),
  the *same one for all three children* so they can compete. Completing it earns a sticker pack and
  builds a **streak** — with bonus packs at 3, 7 and 14 days.
- **Saved World Cup runs** — an unfinished quarter-final is waiting when they next open the app.
- **The album's empty slots** — the most reliable "just one more game" there is.

## Learning content (UK curriculum-flavoured, UK English throughout)

Each player has a **skill rank** — Rookie 🌱 → Pro ⭐ → Star 🌟 → Legend 👑 — earned by answering
correctly. Every rank unlocks harder question types *on top of* the easier ones and makes the
keeper a little sharper, so the game grows with the child instead of running out.

| Player | Maths (grows with rank) | Other |
|--------|-------------------------|-------|
| Ezra (6)  | Sums & subtraction → number bonds, doubles/halves, sequences → 2/5/10 times tables, clock times, coins → sums to 50, three-number addition | Word-to-picture, 2D shapes, first facts |
| Avery (10)| Times tables, fractions → division, decimals, perimeter → area, two-step problems, rounding, negatives → 2-digit multiplication, equivalent fractions, averages | UK geography & science (40 facts) |
| Sols (12) | BODMAS, algebra, percentages → squares/cubes, ratio, negatives → brackets, percentage change, primes, HCF/LCM → index laws, probability, two-step algebra | General knowledge (40 facts) |

There are around **190 different question templates** in total. The keeper also gets sharper the
longer your scoring streak — hat-tricks must be earned.

**Targeted practice.** Every question is tagged by topic and the app tracks accuracy for each one.
Roughly a third of questions are then drawn from the topics a child keeps getting wrong, so weak
spots get extra practice without the game ever feeling like a drill.

## For grown-ups

A **👨‍👩‍👧 Grown-ups** button on the player-select screen (behind a small maths gate, to keep little
ones out) opens a progress dashboard: for each child, their rank, questions answered, overall
accuracy, time played, matches and cups — plus **accuracy broken down by topic**, sorted worst
first, with their weakest and strongest areas called out. It tells you exactly what to help with.

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
