# The Reader — Rider Waite Smith Tarot

A structured tarot learning app built for the browser, designed to take you from first card to full reading. Saveable as a home screen web app on iOS and Android.

Code created by Claude.

---

## What it is

Most tarot apps teach cards in isolation — name, symbol, keyword, next. The Reader is built differently. The spread is the primary unit of learning, not the card. You encounter cards in context, in relationship to one another and to a positional meaning, which is how reading actually works.

The app covers the full 78-card Rider Waite Smith deck with content written at depth: upright and reversed meanings, relational notes for how each card shifts in combination with others, and scenario readings across love, work, and self.

---

## Features

**Diagnostic assessment**
Before anything else, the app tests the quality of your existing understanding — not just whether you recognise card names, but whether you can read positionally and relationally. It outputs a learning profile and sets your starting point accordingly.

**Two learning paths**
- *Foundation* — upright cards only, recommended for beginners
- *Advanced* — upright and reversed, for those ready for the added complexity

**Spread-first practice**
Three spreads available: Three Card (Past / Present / Future), Situation & Path, and Mind / Body / Spirit. Cards are drawn from your unlocked pool. Tapping a position reveals the card with its meaning in context, plus relational notes and a direct link to the full flashcard.

**Card library**
All 78 cards browsable by suit, with locked / unlocked / mastered status. Each card opens a flippable flashcard showing keywords on the front and full meaning, reversed reading, relational notes, and three life scenario panels on the back.

**Quiz modes**
Card meaning quiz and card pairing quiz, both drawing from your unlocked cards. Results tracked over time.

**Reading simulator**
Guided reading scenarios with a real querrant context and a full spread laid out. Rather than open-ended interpretation, the simulator walks you through a sequence of directed questions — teaching the reasoning process a reader actually uses, not just the card meanings.

**Cross-device progress sync**
Progress is stored locally and optionally synced to a `progress.json` file in this GitHub repository via the GitHub API. Enter a personal access token once per device and your profile, unlocked cards, mastered cards, and history stay in step across phone and laptop.

---

## Card images

The app is designed to display Rider Waite Smith card images loaded from a `/cards/` folder in the repository. Images are included here as the original 1909 deck is in the public domain, and scans are widely available. The naming convention expected is:

| Suit | Format | Example |
|------|--------|---------|
| Major Arcana | `m00.jpg` – `m21.jpg` | `m00.jpg` = The Fool |
| Cups | `c01.jpg` – `c14.jpg` | `c01.jpg` = Ace of Cups |
| Wands | `w01.jpg` – `w14.jpg` | `w01.jpg` = Ace of Wands |
| Swords | `s01.jpg` – `s14.jpg` | `s01.jpg` = Ace of Swords |
| Pentacles | `p01.jpg` – `p14.jpg` | `p01.jpg` = Ace of Pentacles |

Court cards follow the same sequence: 11 = Page, 12 = Knight, 13 = Queen, 14 = King.

The app falls back to symbolic emoji for any card image not found, so the folder can be populated gradually.

---

## Installing as a home screen app

Open the GitHub Pages URL in Safari (iOS) or Chrome (Android), then:

- **iOS**: Share → Add to Home Screen
- **Android**: Chrome menu → Add to Home Screen, or accept the install prompt

The app will appear with its own icon and open full-screen without browser chrome.

---

## GitHub Pages URL

[https://pedrowow.github.io/tarot-learning](https://pedrowow.github.io/tarot-learning)

---

## Credit

Deck: Rider Waite Smith Tarot, 1909. Art by **Pamela Colman Smith**, commissioned by Arthur Edward Waite. Published by the Rider Company. Pamela Colman Smith painted all 78 cards and was the first artist to illustrate the full Minor Arcana with narrative scenes — a decision that transformed how tarot is read. She received no royalties and was uncredited on the original publication.
