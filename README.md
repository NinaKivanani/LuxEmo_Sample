# LuxEmo: Expressive Text-to-Speech Corpus for Luxembourgish

**Audio Samples and Subjective Evaluation Demo**

> **Paper:** *LuxEmo: Expressive Text-to-Speech Corpus for Luxembourgish* (Interspeech 2026)

---

## Overview

LuxEmo is a spontaneous emotional speech corpus and benchmark for Luxembourgish text-to-speech (TTS), built from RTL Youth broadcasts. It comprises **21.0 hours** of wideband speech and **7,562 ten-second segments** from four speakers, annotated for language, speaker identity, and four emotion categories (neutral, happy, sad, angry) in a heavily code-switching setting.

This page provides representative audio samples from the five TTS systems evaluated in the paper, organized by target emotion. Listeners can compare models side by side.

**For the full interactive demo with embedded audio players, visit the [GitHub Pages demo](https://ninakivanani.github.io/LuxEmo_Sample/).**

---

## TTS Systems

| Model | Architecture | Language | Emotion Control |
|-------|-------------|----------|-----------------|
| **GradTTS** (de) | Diffusion-based | German (zero-shot) | Reference audio |
| **XTTS** (de) | XTTSv2, cross-lingual | German (zero-shot) | Reference audio |
| **Toucan** (lb) | Reference encoder, multilingual | Luxembourgish | Reference vector |
| **Qwen3_FT** (lb) | LLM-native, per-speaker fine-tuned | Luxembourgish | Prompt-based |
| **kNN TTS** (lb) | GlowTTS + SSL features | Luxembourgish | kNN prosody transfer |

---

## Sample Organization

Samples are organized by model and target emotion:

```
Samples/
├── GradTTS/
│   ├── neutral/    (4 speakers)
│   ├── happy/      (4 speakers)
│   ├── sad/        (4 speakers)
│   └── angry/      (2 speakers)
├── XTTS/
│   ├── neutral/    (4 speakers)
│   ├── happy/      (4 speakers)
│   ├── sad/        (4 speakers)
│   └── angry/      (2 speakers)
├── Toucan/
│   ├── neutral/    (4 speakers)
│   ├── happy/      (4 speakers)
│   ├── sad/        (4 speakers)
│   └── angry/      (2 speakers)
├── Qwen3_FT/
│   ├── neutral/    (4 speakers)
│   └── happy/      (4 speakers)
└── kNN_TTS/
    ├── neutral/    (4 speakers)
    ├── happy/      (4 speakers)
    ├── sad/        (4 speakers)
    └── angry/      (2 speakers)
```

> **Note:** Angry samples are limited because anger covers only 0.5% of the LuxEmo corpus. Qwen3_FT was fine-tuned with prompt-based emotion control for neutral and happy.

---

## Human Evaluation Protocol

The subjective evaluation used a stratified listening test with ten native Luxembourgish listeners. For each audio sample, listeners answered the following:

### A. Emotion Recognition
- **Q1.** Identify the primary emotion expressed in this audio. *(Angry / Happy / Neutral / Sad / Other)*
- **Q2.** How intense is the emotion in this audio? *(1 = None ... 5 = Very strong)*

### B. Emotion Authenticity
- **Q3.** The speaker sounds [target emotion]. *(1 = Strongly disagree ... 5 = Strongly agree)*
- **Q4.** The emotion is conveyed convincingly. *(1 = Strongly disagree ... 5 = Strongly agree)*
- **Q5.** The emotional tone matches the text content. *(1 = Strongly disagree ... 5 = Strongly agree)*

### C. Speech Quality
- **Q6.** How expressive is this audio sample? *(1 = Bad ... 5 = Excellent)*
- **Q7.** How natural does the speech sound? *(1 = Bad ... 5 = Excellent)*
- **Q8.** How clear and intelligible is the speech? *(1 = Bad ... 5 = Excellent)*
- **Q9.** Rate the overall speech quality. *(1 = Bad ... 5 = Excellent)*

### D. Overall Impression
- **Q10.** I would believe this is a real human speaker. *(1 = Strongly disagree ... 5 = Strongly agree)*

---

## Corpus Statistics

| Speaker | Gender | Segments | Duration (min) | Neutral | Happy | Sad | Angry |
|---------|--------|----------|----------------|---------|-------|-----|-------|
| Spk1 | M | 1,240 | 206.7 | 88 | 1,125 | 17 | 10 |
| Spk2 | F | 766 | 127.7 | 190 | 476 | 100 | 0 |
| Spk3 | F | 3,577 | 596.2 | 1,627 | 1,223 | 702 | 25 |
| Spk4 | F | 1,979 | 329.8 | 1,063 | 836 | 77 | 3 |
| **Total** | **1M, 3F** | **7,562** | **1,260.4** | **2,968** | **3,660** | **896** | **38** |

---

## Key Results

| Model | WV MOS | LuxASR WER | Speaker Sim | F0 RMSE |
|-------|--------|------------|-------------|---------|
| GradTTS (de) | 3.891 | 1.721 | 0.172 | 63.0 |
| XTTS (de) | 3.515 | 1.107 | **0.317** | 80.5 |
| Toucan (lb) | 3.498 | **0.832** | 0.224 | 79.8 |
| Qwen3_FT (lb) | 3.357 | 13.263 | 0.315 | 133.0 |
| kNN TTS (lb) | 0.920 | 1.807 | 0.114 | 64.2 |

**Subjective Results (5-point MOS):**

| Model | Naturalness | Emotion Match |
|-------|-------------|---------------|
| Qwen3_FT (lb) | **3.9** | **4.0** |
| Toucan (lb) | 3.7 | 3.8 |
| GradTTS (de) | 3.7 | 3.6 |
| XTTS (de) | 3.4 | 3.4 |
| kNN TTS (lb) | 2.3 | 2.4 |

---

## How to Listen and Evaluate

1. **Visit the [demo page](https://ninakivanani.github.io/LuxEmo_Sample/)** for an interactive listening experience with embedded audio players.
2. Or browse the `Samples/` folder directly and download individual WAV files.
3. For each sample, consider the evaluation questions listed above.

---

## License

This repository contains synthesized audio samples only. The LuxEmo corpus itself is constructed from RTL broadcasts and cannot be publicly redistributed due to licensing constraints. All data were collected with prior speaker consent and in compliance with applicable EU privacy regulations.

MIT License applies to the code and sample page in this repository.
