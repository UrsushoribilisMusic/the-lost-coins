# The Lost Coins

A SciFi thriller serialised on Substack. Crypto, cryonics, cartels, and two women who didn't plan on any of it.

**Read the full story**: [scifibymiguel.substack.com](https://scifibymiguel.substack.com)

---

## What is this repository?

This repo contains the full production archive for *The Lost Coins* — every chapter's prose text, Runway video prompts, Suno AI music styles, TikTok/YouTube captions, and chapter artwork.

It does **not** contain video or audio files (those live on YouTube and TikTok).

---

## Story

A Swiss crypto hacker, a neuroscientist, and a mysterious fixer are hired to recover a legendary lost Bitcoin wallet — the one belonging to Hal Finney, the first person Satoshi Nakamoto ever sent Bitcoin to, now cryogenically preserved in a facility in Arizona.

Behind them: a Macau crime boss who wants to own the room, not just pass through it. A Mexican cartel operator with a portable lab hidden in a Sequoia forest. And two Swiss police inspectors who decide the best move is to let them fly.

~48 chapters. Three acts. One twist nobody sees coming.

---

## Repository Structure

```
the-lost-coins/
├── README.md
├── characters.md          Character profiles and physical descriptions
├── story_outline.md       Full arc: Ch0–47, act structure, key plot points
├── the_lost_coins_full.txt  Consolidated prose Ch0–38
└── chapters/
    ├── ch00/
    │   ├── text.txt       Chapter prose
    │   ├── prompts.txt    Runway veo3 video prompts (4 per chapter)
    │   ├── suno_styles.txt  Suno AI music style descriptions (3 per chapter)
    │   ├── captions.txt   TikTok/YouTube couplet captions
    │   ├── lyrics.txt     Song lyrics (Ch1–9)
    │   └── artwork.jpg    Chapter artwork 1600×900 (Ch1–8)
    ├── ch01/
    │   └── ...
    └── ch38/
```

---

## Production Pipeline

Each chapter goes through this pipeline before publishing to TikTok and YouTube:

```
Text → Runway Prompts → Suno Styles → Lyrics
         ↓                  ↓
    Runway veo3         Suno Audio
    (4 × 8s clips)      (MP3)
         ↓                  ↓
         └──── Video Assembly (9:16 vertical) ────┘
                          ↓
              TikTok / YouTube Shorts
```

Video clip generation uses the **Runway veo3** model. Prompts are kept under 1000 characters and use side/back angles to avoid face inconsistency across clips.

Music is generated with **Suno AI** — styles are matched to the chapter's dominant character and mood (Chinese Erhu for Zheng scenes, Ranchera for Gonzales, folk/Bossa Nova for Napa, Country Noir for FBI).

---

## Character Quick Reference

| Character | Role | Appearance |
|-----------|------|------------|
| Lena Vance | Scout / double agent | Long blonde hair, blue eyes, charcoal blazer |
| Paul Arndt | Crypto hacker | Dark curly hair, hoodie, stubble |
| Erica Voss | Neuroscientist | Long dark hair, brown eyes, white lab coat |
| Mr. Zheng | Macau crime boss | Silver-streaked hair, tailored charcoal suit |
| Gonzales ("Speedy") | Cartel operator | Heavyset, salt-and-pepper mustache |
| Inspector Pinto | FBI / Interpol | The vendetta behind the badge |

Full profiles in [characters.md](./characters.md).

---

## Status

- **Ch0–38**: Prose written, prompts + captions generated
- **Ch1–8**: Full production complete (video published)
- **Ch9**: Runway clips generated, final video published
- **Ch10–24**: Text + prompts complete; need audio → clips → final video
- **Ch25–38**: Text + prompts complete; need audio → clips → final video
- **Ch39–47**: Outline only; prose to be written
