# LuxEmo: Expressive Text-to-Speech Corpus for Luxembourgish

**Audio Samples and Subjective Evaluation**

> *LuxEmo: Expressive Text-to-Speech Corpus for Luxembourgish* — Interspeech 2026

---

## Overview

LuxEmo is a spontaneous emotional speech corpus and benchmark for Luxembourgish TTS, built from RTL Youth broadcasts. It comprises **21.0 hours** of wideband speech and **7,562 ten-second segments** from four speakers, annotated for four emotions (neutral, happy, sad, angry) in a heavily code-switching setting.

This repository provides **64 synthesized audio samples** from five TTS systems for side-by-side comparison. Browse the `Samples/` folder to download and listen.

---

## TTS Systems

| # | Model | Architecture | Language | Emotion Control |
|:-:|-------|-------------|----------|-----------------|
| 1 | **GradTTS** | Diffusion-based | German (zero-shot) | Reference audio |
| 2 | **XTTS** | XTTSv2, cross-lingual | German (zero-shot) | Reference audio |
| 3 | **Toucan** | Reference encoder | Luxembourgish | Reference vector |
| 4 | **Qwen3\_FT** | LLM-native, fine-tuned | Luxembourgish | Prompt-based |
| 5 | **kNN TTS** | GlowTTS + SSL | Luxembourgish | kNN prosody transfer |

---

## Audio Samples

Samples are organized as `Samples/{Model}/{emotion}/{Speaker}_{emotion}_000.wav`.

### Neutral Samples

> Listen to each model and answer: *What emotion do you hear? How natural does it sound?*

| Speaker | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|---------|:------------:|:---------:|:-----------:|:--------------:|:------------:|
| **Spk1** (M) | [listen](Samples/GradTTS/neutral/Edouard_neutral_000.wav) | [listen](Samples/XTTS/neutral/Edouard_neutral_000.wav) | [listen](Samples/Toucan/neutral/Edouard_neutral_000.wav) | [listen](Samples/Qwen3_FT/neutral/Edouard_neutral_000.wav) | [listen](Samples/kNN_TTS/neutral/Edouard_neutral_000.wav) |
| **Spk3** (F) | [listen](Samples/GradTTS/neutral/Nathalie_Claire_neutral_000.wav) | [listen](Samples/XTTS/neutral/Nathalie_Claire_neutral_000.wav) | [listen](Samples/Toucan/neutral/Nathalie_Claire_neutral_000.wav) | [listen](Samples/Qwen3_FT/neutral/Nathalie_Claire_neutral_000.wav) | [listen](Samples/kNN_TTS/neutral/Nathalie_Claire_neutral_000.wav) |
| **Spk2** (F) | [listen](Samples/GradTTS/neutral/Sarah_neutral_000.wav) | [listen](Samples/XTTS/neutral/Sarah_neutral_000.wav) | [listen](Samples/Toucan/neutral/Sarah_neutral_000.wav) | [listen](Samples/Qwen3_FT/neutral/Sarah_neutral_000.wav) | [listen](Samples/kNN_TTS/neutral/Sarah_neutral_000.wav) |
| **Spk4** (F) | [listen](Samples/GradTTS/neutral/Mandy_Hufflepuff_neutral_000.wav) | [listen](Samples/XTTS/neutral/Mandy_Hufflepuff_neutral_000.wav) | [listen](Samples/Toucan/neutral/Mandy_Hufflepuff_neutral_000.wav) | [listen](Samples/Qwen3_FT/neutral/Mandy_Hufflepuff_neutral_000.wav) | [listen](Samples/kNN_TTS/neutral/Mandy_Hufflepuff_neutral_000.wav) |

### Happy Samples

> *The speaker sounds happy — do you agree? Rate 1–5. How expressive is this audio?*

| Speaker | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|---------|:------------:|:---------:|:-----------:|:--------------:|:------------:|
| **Spk1** (M) | [listen](Samples/GradTTS/happy/Edouard_happy_000.wav) | [listen](Samples/XTTS/happy/Edouard_happy_000.wav) | [listen](Samples/Toucan/happy/Edouard_happy_000.wav) | [listen](Samples/Qwen3_FT/happy/Edouard_happy_000.wav) | [listen](Samples/kNN_TTS/happy/Edouard_happy_000.wav) |
| **Spk3** (F) | [listen](Samples/GradTTS/happy/Nathalie_Claire_happy_000.wav) | [listen](Samples/XTTS/happy/Nathalie_Claire_happy_000.wav) | [listen](Samples/Toucan/happy/Nathalie_Claire_happy_000.wav) | [listen](Samples/Qwen3_FT/happy/Nathalie_Claire_happy_000.wav) | [listen](Samples/kNN_TTS/happy/Nathalie_Claire_happy_000.wav) |
| **Spk2** (F) | [listen](Samples/GradTTS/happy/Sarah_happy_000.wav) | [listen](Samples/XTTS/happy/Sarah_happy_000.wav) | [listen](Samples/Toucan/happy/Sarah_happy_000.wav) | [listen](Samples/Qwen3_FT/happy/Sarah_happy_000.wav) | [listen](Samples/kNN_TTS/happy/Sarah_happy_000.wav) |
| **Spk4** (F) | [listen](Samples/GradTTS/happy/Mandy_Hufflepuff_happy_000.wav) | [listen](Samples/XTTS/happy/Mandy_Hufflepuff_happy_000.wav) | [listen](Samples/Toucan/happy/Mandy_Hufflepuff_happy_000.wav) | [listen](Samples/Qwen3_FT/happy/Mandy_Hufflepuff_happy_000.wav) | [listen](Samples/kNN_TTS/happy/Mandy_Hufflepuff_happy_000.wav) |

### Sad Samples

> *The speaker sounds sad — do you agree? Does the emotional tone match the text content?*

| Speaker | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|---------|:------------:|:---------:|:-----------:|:--------------:|:------------:|
| **Spk1** (M) | [listen](Samples/GradTTS/sad/Edouard_sad_000.wav) | [listen](Samples/XTTS/sad/Edouard_sad_000.wav) | [listen](Samples/Toucan/sad/Edouard_sad_000.wav) | — | [listen](Samples/kNN_TTS/sad/Edouard_sad_000.wav) |
| **Spk3** (F) | [listen](Samples/GradTTS/sad/Nathalie_Claire_sad_000.wav) | [listen](Samples/XTTS/sad/Nathalie_Claire_sad_000.wav) | [listen](Samples/Toucan/sad/Nathalie_Claire_sad_000.wav) | — | [listen](Samples/kNN_TTS/sad/Nathalie_Claire_sad_000.wav) |
| **Spk2** (F) | [listen](Samples/GradTTS/sad/Sarah_sad_000.wav) | [listen](Samples/XTTS/sad/Sarah_sad_000.wav) | [listen](Samples/Toucan/sad/Sarah_sad_000.wav) | — | [listen](Samples/kNN_TTS/sad/Sarah_sad_000.wav) |
| **Spk4** (F) | [listen](Samples/GradTTS/sad/Mandy_Hufflepuff_sad_000.wav) | [listen](Samples/XTTS/sad/Mandy_Hufflepuff_sad_000.wav) | [listen](Samples/Toucan/sad/Mandy_Hufflepuff_sad_000.wav) | — | [listen](Samples/kNN_TTS/sad/Mandy_Hufflepuff_sad_000.wav) |

> Qwen3\_FT was fine-tuned for neutral and happy only; no sad samples available.

### Angry Samples

> *The speaker sounds angry — do you agree? How intense is the emotion? (Anger = 0.5% of the corpus)*

| Speaker | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|---------|:------------:|:---------:|:-----------:|:--------------:|:------------:|
| **Spk3** (F) | [listen](Samples/GradTTS/angry/Nathalie_Claire_angry_000.wav) | [listen](Samples/XTTS/angry/Nathalie_Claire_angry_000.wav) | [listen](Samples/Toucan/angry/Nathalie_Claire_angry_000.wav) | — | [listen](Samples/kNN_TTS/angry/Nathalie_Claire_angry_000.wav) |
| **Spk2** (F) | [listen](Samples/GradTTS/angry/Sarah_angry_000.wav) | [listen](Samples/XTTS/angry/Sarah_angry_000.wav) | [listen](Samples/Toucan/angry/Sarah_angry_000.wav) | — | [listen](Samples/kNN_TTS/angry/Sarah_angry_000.wav) |

> Angry is the rarest category (38 segments, 0.5%). Samples available from two speakers only.

---

## Human Evaluation Protocol

The subjective evaluation used a stratified listening test with **ten native Luxembourgish listeners** (ages 20–50, balanced gender, self-reported normal hearing). Each session lasted 12–15 minutes.

<details>
<summary><strong>A. Emotion Recognition (Q1–Q2)</strong></summary>

| # | Question | Scale |
|:-:|----------|-------|
| Q1 | **Identify the primary emotion expressed in this audio.** | A. Happy · B. Neutral · C. Sad · D. Angry · E. Other/Unsure |
| Q2 | **How intense is the emotion in this audio?** | 1 = None · 2 = Slight · 3 = Moderate · 4 = Strong · 5 = Very strong |

</details>

<details>
<summary><strong>B. Emotion Authenticity (Q3–Q5)</strong></summary>

| # | Question | Scale |
|:-:|----------|-------|
| Q3 | **The speaker sounds [target emotion].** | 1 = Strongly disagree · · · 5 = Strongly agree |
| Q4 | **The emotion is conveyed convincingly.** | 1 = Strongly disagree · · · 5 = Strongly agree |
| Q5 | **Does the emotional tone match the text content?** | 1 = Strongly disagree · · · 5 = Strongly agree |

</details>

<details>
<summary><strong>C. Speech Quality (Q6–Q9)</strong></summary>

| # | Question | Scale |
|:-:|----------|-------|
| Q6 | **How expressive do you find this audio sample?** | 1 = Bad · 2 = Poor · 3 = Fair · 4 = Good · 5 = Excellent |
| Q7 | **How natural does the speech sound?** | 1 = Bad · · · 5 = Excellent |
| Q8 | **How clear and intelligible is the speech?** | 1 = Bad · · · 5 = Excellent |
| Q9 | **Rate the overall speech quality.** | 1 = Bad · · · 5 = Excellent |

</details>

<details>
<summary><strong>D. Overall Impression (Q10)</strong></summary>

| # | Question | Scale |
|:-:|----------|-------|
| Q10 | **I would believe this is a real human speaker.** | 1 = Strongly disagree · · · 5 = Strongly agree |

</details>

---

## Key Results

### Objective Metrics

| Model | WV MOS ↑ | LuxASR WER ↓ | Speaker Sim ↑ | F0 RMSE ↓ |
|-------|:--------:|:------------:|:-------------:|:---------:|
| GradTTS (de) | **3.891** | 1.721 | 0.172 | 63.0 |
| XTTS (de) | 3.515 | 1.107 | **0.317** | 80.5 |
| Toucan (lb) | 3.498 | **0.832** | 0.224 | 79.8 |
| Qwen3\_FT (lb) | 3.357 | 13.263 | 0.315 | 133.0 |
| kNN TTS (lb) | 0.920 | 1.807 | 0.114 | **64.2** |

> ↑ higher is better · ↓ lower is better · **bold** = best per metric

### Subjective Evaluation (5-point MOS)

| Model | Naturalness ↑ | Emotion Match ↑ |
|-------|:-------------:|:---------------:|
| Qwen3\_FT (lb) | **3.9** | **4.0** |
| Toucan (lb) | 3.7 | 3.8 |
| GradTTS (de) | 3.7 | 3.6 |
| XTTS (de) | 3.4 | 3.4 |
| kNN TTS (lb) | 2.3 | 2.4 |

### Emotion Recognition Accuracy

| Emotion | Recognition Rate |
|---------|:----------------:|
| Happy | ~80% |
| Neutral | ~75% |
| Sad | ~65% |
| Angry | ~55% |

> Luxembourgish-adapted models (Qwen3\_FT, Toucan) are preferred over German zero-shot systems by native listeners, demonstrating the value of language-specific training data for emotional TTS.

---

## Corpus Statistics

| Speaker | Gender | Segments | Duration (min) | Neutral | Happy | Sad | Angry |
|:-------:|:------:|:--------:|:--------------:|:-------:|:-----:|:---:|:-----:|
| Spk1 | M | 1,240 | 206.7 | 88 | 1,125 | 17 | 10 |
| Spk2 | F | 766 | 127.7 | 190 | 476 | 100 | 0 |
| Spk3 | F | 3,577 | 596.2 | 1,627 | 1,223 | 702 | 25 |
| Spk4 | F | 1,979 | 329.8 | 1,063 | 836 | 77 | 3 |
| **Total** | **1M, 3F** | **7,562** | **1,260.4** | **2,968** | **3,660** | **896** | **38** |

---

## License

This repository contains synthesized audio samples only. The LuxEmo corpus itself is constructed from RTL broadcasts and cannot be publicly redistributed due to licensing constraints. All data were collected with prior speaker consent and in compliance with applicable EU privacy regulations.
