# Kannada Matras Trainer

A progressive web app (PWA) for practicing Kannada kagunita — consonant + vowel matra combinations — with Devanagari as the answer script. Designed for learners who want reading fluency in Kannada, not academic completeness.

The app works offline, installs to your home screen, and requires no server or build step.

## What it practices

Kannada uses vowel signs (matras) attached to consonants to form syllables. For example:

- ಕ (ka) + ಾ → ಕಾ (kaa) → का
- ಕ (ka) + ಿ → ಕಿ (ki) → कि
- ಕ (ka) + ೈ → ಕೈ (kai) → कै

The deck covers **33 consonants** × **11 matras** (ಾ ಿ ೀ ು ೂ ೆ ೇ ೊ ೋ ೈ ೌ) = ~360 CV cards, plus a small set of single-base matra recognition cards. All answers are in Devanagari, which works well as a bridge script for Hindi/Marathi readers learning Kannada.

## Practice modes

| Mode | What it does |
|---|---|
| **Mixed deck** | Random selection across the full card set |
| **All matras for a random consonant** | Drills all vowel forms of one consonant, e.g. all ಕ forms |
| **All consonants for a random matra** | Drills one matra across all consonants, e.g. all ಾ (aa) forms |
| **Practice Weak Matras** | Targets cards below 99% accuracy (needs ≥ 8 attempts per card first) |

Each session shows multiple-choice options. The **Harder distractor mode** (default) keeps wrong answers within the same consonant family, reducing guesswork.

## Features

- Embedded deck — no CSV file needed to run
- Per-card accuracy tracking persisted in `localStorage`
- Session history with accuracy and response time
- Installable as a PWA on iOS (Safari → Add to Home Screen) and Android
- Keyboard shortcuts: `1` `2` `3` to answer, `Space` to skip

## Files

- `index.html` — the entire app; deck data is embedded here
- `manifest.json` — PWA metadata
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `favicon.png` — app icons
- `kannada_matra_master_v6_1.csv` — source reference for the deck; not required at runtime
- `.nojekyll` — prevents GitHub Pages from processing the repo with Jekyll

## Deploy on GitHub Pages

1. Create a new GitHub repository
2. Upload all files to the repository root
3. Go to **Settings → Pages**
4. Under **Build and deployment**, set:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` (or `master`), folder `/ (root)`
5. Save — GitHub will provide a Pages URL within a minute or two
6. On iPhone: open the URL in Safari → Share → **Add to Home Screen**

## Local use

Open `index.html` directly in any browser — no server needed. Progress is saved in the browser's `localStorage`, so it persists across sessions as long as you use the same browser.

## Companion app

Pairs with the [Kannada Alphabet Trainer(https://github.com/AGPATHAK/alphabet)](https://github.com/AGPATHAK/Kannada_alphabet) which covers base letter recognition before moving on to matras.
