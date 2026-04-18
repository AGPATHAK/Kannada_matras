# Kannada Matras Trainer

A browser-based PWA for practicing Kannada kagunita — consonant + vowel matra combinations — with Devanagari as the answer script. Built for personal practice toward reading fluency — newspapers, simple stories — rather than academic study.

## Live app

[[https://agpathak.github.io/Kannada_matra/](https://agpathak.github.io/Kannada_matra/)](https://agpathak.github.io/Kannada_matras/)

## What it covers

Kannada uses vowel signs (matras) attached to consonants to form syllables. For example:

- ಕ (ka) + ಾ → ಕಾ (kaa) → का
- ಕ (ka) + ಿ → ಕಿ (ki) → कि
- ಕ (ka) + ೈ → ಕೈ (kai) → कै

The deck covers **33 consonants** × **11 matras** (ಾ ಿ ೀ ು ೂ ೆ ೇ ೊ ೋ ೈ ೌ) = ~360 cards. All answers are in Devanagari — a practical bridge for learners who already read Hindi or Marathi.

## Practice modes

| Mode | What it does |
|---|---|
| **Mixed deck** | Random selection across the full card set |
| **All matras for a random consonant** | Drills all vowel forms of one consonant, e.g. all ಕ forms |
| **All consonants for a random matra** | Drills one matra across all consonants, e.g. all ಾ (aa) forms |
| **Practice Weak Matras** | Cards below 99% accuracy (needs ≥ 8 attempts per card) |

The **Harder distractor mode** (default) keeps wrong answers within the same consonant family, reducing guesswork.

## Features

- Embedded deck — no CSV file needed to run
- Per-card accuracy tracking persisted in `localStorage`
- Session history with accuracy and response time
- Wrong-card review at end of each session with retry option
- Keyboard shortcuts: `1` `2` `3` to answer, `Space` to skip
- Installable as a PWA on iOS and Android
- No server, no backend, no build step — one HTML file

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

Open `index.html` directly in any browser — no server needed. Progress is saved in `localStorage` and persists across sessions in the same browser but does not sync across devices.

## Tech

Plain HTML, CSS, and JavaScript. Tailwind CSS via CDN for styling, Noto Sans Kannada via Google Fonts for script rendering. Hosted on GitHub Pages.

## Companion app

Start with the [Kannada Alphabet Trainer](https://github.com/AGPATHAK/Kannada_alphabet) to learn base letter recognition before moving on to matras.
