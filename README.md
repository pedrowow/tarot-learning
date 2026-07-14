# The Reader — Rider Waite Smith Tarot

A structured tarot learning app built for the browser, designed to take you from first card to full reading. A single HTML file, no build step, deployable on GitHub Pages, and saveable as a home screen web app on iOS and Android.

Code created with Claude.

---

## The learning approach

Most tarot apps teach cards in isolation — name, keyword, next — and depend on memorisation. The Reader is built on two different principles.

**Symbols before cards.** The deck's meaning lives in its imagery: the pillars, the white rose, the loose chains, the colour of the sky. The app carries a glossary of 60 recurring symbols across six groups (celestial, nature, creatures, figures, objects, colours), each with its meaning and cross-references to every card that carries it. Because the same symbols repeat across the deck, learning one symbol teaches fragments of many cards at once — and opens up combination reading, since shared symbolism is how cards speak to each other.

**Spreads before flashcards.** Cards are encountered in context: in relationship to a position, to the other cards drawn, and to a synthesis of the whole. Reading is the skill; card recall is only its raw material.

---

## Levels

Progression is self-directed. Four levels are always visible on the dashboard, and you move up or down as you feel ready:

| Level | Cards in play |
|-------|---------------|
| The Seeker | Major Arcana 0–IX |
| The Initiated Reader | All 22 Major Arcana |
| The Adept | Majors plus the numbered Minors, Ace to Ten |
| The Master | The full 78, court cards included |

Your recent quiz accuracy at the current level is shown as guidance — comfortable above 80%, no rush below 60% — but the choice is always yours. Spreads draw from everything your level unlocks; quizzes test the cards classified at your level, so each tier has a distinct focus.

---

## Practice

**Three Card Spread** — Past / Present / Future. **Five Card Spread** — Past / Present / Hidden Influences / Advice / Likely Outcome. All draws are upright.

Each revealed card shows its meaning, and an *In This Context* note that references only cards actually on the table, falling back to a position-aware reading when no cross-reference applies. When the final card turns, a synthesis of the combination is generated from the structured card data: the weight of Majors present, suit dominance, symbols recurring across the draw, repeating numbers, and a narrative arc across the positions. Three-card readings close with a *Reframe It* prompt, re-reading the same draw as Mind / Body / Spirit and Situation / Obstacle / Advice.

---

## Quizzes

Three modes, all scoped to the current level, all feeding the accuracy guidance and the per-level quiz counter:

**Card Meaning Quiz** — match a card to its full keyword set. **Card Pairing Quiz** — identify the dialogue a pair of cards opens; feedback teaches the pair's elemental relationship and any symbols they share. **Symbol Quiz** — shown a card, spot which symbol appears on it (suit emblems excluded — naming the suit is not observation). Feedback gives the symbol's meaning and which other cards at your level carry it.

In any quiz, tapping a card image enlarges it without revealing anything; a separate *Full card* link opens the complete flashcard.

---

## Card library

All 78 cards browsable by suit, each labelled with its home level and starred when mastered. Every card opens a flippable flashcard: keywords and zoomable image on the front; upright, reversed, and combination meanings on the back; plus tappable symbol chips and scenario readings for love, work, and self. A Symbols tab lists the full glossary — each symbol opens a panel with its meaning and thumbnails of every card that carries it.

---

## Progress and sync

The app is free to use by anyone at the URL below. Progress — level, mastered cards, quiz history, spread counts — is saved automatically in the browser's localStorage, per device, with no account needed. Clearing browser data clears progress.

Cross-device sync is an owner-only feature: it writes progress to `progress.json` in this repository via the GitHub API, so it works only with a personal access token for the repository owner's account (classic token, `repo` scope only). The token is stored solely in the browser's localStorage and transmitted only to `api.github.com`. Visitors can simply tap *Continue* on the setup screen. The repository is public because GitHub Pages requires it on a free plan — the only personal data it contains is the owner's own learning progress.

A *Reset All Progress* option lives on the Sync Setup screen (tap the sync bar on the dashboard). It wipes progress locally and on GitHub in one confirmed action, and stamps a reset epoch so other devices adopt the clean slate on their next sync rather than resurrecting old history. The token survives a reset.

---

## Card images

Rider Waite Smith card images load from the `/cards/` folder — included here as the original 1909 deck is in the public domain. Naming convention:

| Suit | Format | Example |
|------|--------|---------|
| Major Arcana | `m00.jpg` – `m21.jpg` | `m00.jpg` = The Fool |
| Cups | `c01.jpg` – `c14.jpg` | `c01.jpg` = Ace of Cups |
| Wands | `w01.jpg` – `w14.jpg` | `w01.jpg` = Ace of Wands |
| Swords | `s01.jpg` – `s14.jpg` | `s01.jpg` = Ace of Swords |
| Pentacles | `p01.jpg` – `p14.jpg` | `p01.jpg` = Ace of Pentacles |

Court cards follow the same sequence: 11 = Page, 12 = Knight, 13 = Queen, 14 = King. If a local image is missing (for instance when running the file standalone), the app retries from the deployed GitHub Pages site before falling back to a symbolic emoji.

---

## Installing as a home screen app

Open the GitHub Pages URL in Safari (iOS) or Chrome (Android), then:

- **iOS**: Share → Add to Home Screen
- **Android**: Chrome menu → Add to Home Screen, or accept the install prompt

The app opens full-screen with its own icon, without browser chrome.

---

## GitHub Pages URL

[https://pedrowow.github.io/tarot-learning](https://pedrowow.github.io/tarot-learning)

---

## Credit

Deck: Rider Waite Smith Tarot, 1909. Art by **Pamela Colman Smith**, commissioned by Arthur Edward Waite. Published by the Rider Company. Pamela Colman Smith painted all 78 cards and was the first artist to illustrate the full Minor Arcana with narrative scenes — a decision that transformed how tarot is read. She received no royalties and was uncredited on the original publication.
