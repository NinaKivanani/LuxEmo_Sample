# LuxEmo: Expressive Text-to-Speech Corpus for Luxembourgish

**Synthesized audio samples accompanying the Interspeech 2026 submission.**

LuxEmo is a spontaneous emotional speech corpus and benchmark for Luxembourgish TTS, built from RTL Youth broadcasts. It comprises 21.0 hours of wideband speech (7,562 ten-second segments) from four speakers, annotated for four emotions (neutral, happy, sad, angry) in a code-switching setting. We benchmark five expressive TTS systems covering zero-shot multilingual, cross-lingual, and Luxembourgish-adapted strategies.

---

## TTS Systems (Table in Section 3)

| Model | Base | Lux FT | Emotion control | Lang |
|:------|:-----|:------:|:----------------|:----:|
| GradTTS | GradTTS | -- | ref audio | de |
| XTTS | XTTSv2 | -- | ref audio | de |
| Toucan | Toucan | -- | ref vec | lb |
| Qwen3\_FT | Qwen3 | yes | prompt | lb |
| kNN TTS | GlowTTS+SSL | yes | retrieved prosody | lb |

GradTTS and XTTS use German as a proxy language (de); Toucan uses a multilingual phoneme inventory covering Luxembourgish (lb); Qwen3\_FT is per-speaker fine-tuned on LuxEmo with prompt-based emotion control; kNN TTS transfers prosody via k-nearest-neighbor retrieval from LuxEmo segments.

---

## Audio Samples

Representative synthesized samples for each system and target emotion. For the subjective evaluation, listeners assessed each sample on three dimensions:

1. **Perceived emotion** — Neutral / Happy / Sad / Angry / Other
2. **Emotion intensity** — 1 (none) to 5 (very strong)
3. **Naturalness & appropriateness** — 1 (poor) to 5 (excellent)

### Neutral — Spk3 (F)

**GradTTS (de)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/GradTTS/neutral/Spk3_neutral_000.mp4

**XTTS (de)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/XTTS/neutral/Spk3_neutral_000.mp4

**Toucan (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/Toucan/neutral/Spk3_neutral_000.mp4

**Qwen3\_FT (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/Qwen3_FT/neutral/Spk3_neutral_000.mp4

**kNN TTS (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/kNN_TTS/neutral/Spk3_neutral_000.mp4

<details><summary>All speakers — Neutral (download wav)</summary>

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| Spk1 (M) | [wav](Samples/GradTTS/neutral/Spk1_neutral_000.wav) | [wav](Samples/XTTS/neutral/Spk1_neutral_000.wav) | [wav](Samples/Toucan/neutral/Spk1_neutral_000.wav) | [wav](Samples/Qwen3_FT/neutral/Spk1_neutral_000.wav) | [wav](Samples/kNN_TTS/neutral/Spk1_neutral_000.wav) |
| Spk2 (F) | [wav](Samples/GradTTS/neutral/Spk2_neutral_000.wav) | [wav](Samples/XTTS/neutral/Spk2_neutral_000.wav) | [wav](Samples/Toucan/neutral/Spk2_neutral_000.wav) | [wav](Samples/Qwen3_FT/neutral/Spk2_neutral_000.wav) | [wav](Samples/kNN_TTS/neutral/Spk2_neutral_000.wav) |
| Spk3 (F) | [wav](Samples/GradTTS/neutral/Spk3_neutral_000.wav) | [wav](Samples/XTTS/neutral/Spk3_neutral_000.wav) | [wav](Samples/Toucan/neutral/Spk3_neutral_000.wav) | [wav](Samples/Qwen3_FT/neutral/Spk3_neutral_000.wav) | [wav](Samples/kNN_TTS/neutral/Spk3_neutral_000.wav) |
| Spk4 (F) | [wav](Samples/GradTTS/neutral/Spk4_neutral_000.wav) | [wav](Samples/XTTS/neutral/Spk4_neutral_000.wav) | [wav](Samples/Toucan/neutral/Spk4_neutral_000.wav) | [wav](Samples/Qwen3_FT/neutral/Spk4_neutral_000.wav) | [wav](Samples/kNN_TTS/neutral/Spk4_neutral_000.wav) |

</details>

---

### Happy — Spk3 (F)

**GradTTS (de)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/GradTTS/happy/Spk3_happy_000.mp4

**XTTS (de)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/XTTS/happy/Spk3_happy_000.mp4

**Toucan (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/Toucan/happy/Spk3_happy_000.mp4

**Qwen3\_FT (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/Qwen3_FT/happy/Spk3_happy_000.mp4

**kNN TTS (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/kNN_TTS/happy/Spk3_happy_000.mp4

<details><summary>All speakers — Happy (download wav)</summary>

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| Spk1 (M) | [wav](Samples/GradTTS/happy/Spk1_happy_000.wav) | [wav](Samples/XTTS/happy/Spk1_happy_000.wav) | [wav](Samples/Toucan/happy/Spk1_happy_000.wav) | [wav](Samples/Qwen3_FT/happy/Spk1_happy_000.wav) | [wav](Samples/kNN_TTS/happy/Spk1_happy_000.wav) |
| Spk2 (F) | [wav](Samples/GradTTS/happy/Spk2_happy_000.wav) | [wav](Samples/XTTS/happy/Spk2_happy_000.wav) | [wav](Samples/Toucan/happy/Spk2_happy_000.wav) | [wav](Samples/Qwen3_FT/happy/Spk2_happy_000.wav) | [wav](Samples/kNN_TTS/happy/Spk2_happy_000.wav) |
| Spk3 (F) | [wav](Samples/GradTTS/happy/Spk3_happy_000.wav) | [wav](Samples/XTTS/happy/Spk3_happy_000.wav) | [wav](Samples/Toucan/happy/Spk3_happy_000.wav) | [wav](Samples/Qwen3_FT/happy/Spk3_happy_000.wav) | [wav](Samples/kNN_TTS/happy/Spk3_happy_000.wav) |
| Spk4 (F) | [wav](Samples/GradTTS/happy/Spk4_happy_000.wav) | [wav](Samples/XTTS/happy/Spk4_happy_000.wav) | [wav](Samples/Toucan/happy/Spk4_happy_000.wav) | [wav](Samples/Qwen3_FT/happy/Spk4_happy_000.wav) | [wav](Samples/kNN_TTS/happy/Spk4_happy_000.wav) |

</details>

---

### Sad — Spk3 (F)

**GradTTS (de)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/GradTTS/sad/Spk3_sad_000.mp4

**XTTS (de)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/XTTS/sad/Spk3_sad_000.mp4

**Toucan (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/Toucan/sad/Spk3_sad_000.mp4

**Qwen3\_FT (lb)** — not available (fine-tuned for neutral and happy only)

**kNN TTS (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/kNN_TTS/sad/Spk3_sad_000.mp4

<details><summary>All speakers — Sad (download wav)</summary>

| | GradTTS (de) | XTTS (de) | Toucan (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|
| Spk1 (M) | [wav](Samples/GradTTS/sad/Spk1_sad_000.wav) | [wav](Samples/XTTS/sad/Spk1_sad_000.wav) | [wav](Samples/Toucan/sad/Spk1_sad_000.wav) | [wav](Samples/kNN_TTS/sad/Spk1_sad_000.wav) |
| Spk2 (F) | [wav](Samples/GradTTS/sad/Spk2_sad_000.wav) | [wav](Samples/XTTS/sad/Spk2_sad_000.wav) | [wav](Samples/Toucan/sad/Spk2_sad_000.wav) | [wav](Samples/kNN_TTS/sad/Spk2_sad_000.wav) |
| Spk3 (F) | [wav](Samples/GradTTS/sad/Spk3_sad_000.wav) | [wav](Samples/XTTS/sad/Spk3_sad_000.wav) | [wav](Samples/Toucan/sad/Spk3_sad_000.wav) | [wav](Samples/kNN_TTS/sad/Spk3_sad_000.wav) |
| Spk4 (F) | [wav](Samples/GradTTS/sad/Spk4_sad_000.wav) | [wav](Samples/XTTS/sad/Spk4_sad_000.wav) | [wav](Samples/Toucan/sad/Spk4_sad_000.wav) | [wav](Samples/kNN_TTS/sad/Spk4_sad_000.wav) |

</details>

---

### Angry — Spk3 (F)

Anger is the rarest emotion in LuxEmo (0.5% of segments, 38 total).

**GradTTS (de)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/GradTTS/angry/Spk3_angry_000.mp4

**XTTS (de)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/XTTS/angry/Spk3_angry_000.mp4

**Toucan (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/Toucan/angry/Spk3_angry_000.mp4

**Qwen3\_FT (lb)** — not available

**kNN TTS (lb)**

https://github.com/NinaKivanani/LuxEmo_Sample/raw/main/Samples/kNN_TTS/angry/Spk3_angry_000.mp4

<details><summary>All speakers — Angry (download wav)</summary>

| | GradTTS (de) | XTTS (de) | Toucan (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|
| Spk2 (F) | [wav](Samples/GradTTS/angry/Spk2_angry_000.wav) | [wav](Samples/XTTS/angry/Spk2_angry_000.wav) | [wav](Samples/Toucan/angry/Spk2_angry_000.wav) | [wav](Samples/kNN_TTS/angry/Spk2_angry_000.wav) |
| Spk3 (F) | [wav](Samples/GradTTS/angry/Spk3_angry_000.wav) | [wav](Samples/XTTS/angry/Spk3_angry_000.wav) | [wav](Samples/Toucan/angry/Spk3_angry_000.wav) | [wav](Samples/kNN_TTS/angry/Spk3_angry_000.wav) |

</details>

---

## Objective Evaluation Results (Section 4)

Higher WV MOS and CosSim indicate better performance; lower WER and F0 RMSE indicate better performance.

| Model | Lang / training | WV MOS | WER\_Lux | CosSim | F0 RMSE |
|:------|:----------------|:------:|:--------:|:------:|:-------:|
| *Acted German reference* | | | | | |
| GradTTS (EmoDB) | de, acted | **4.166** | — | 0.226 | **44.2** |
| *Zero-shot baselines* | | | | | |
| GradTTS (de) | de, zero-shot | 3.891 | 1.721 | 0.172 | 63.0 |
| XTTS (de) | de, zero-shot | 3.515 | 1.107 | **0.317** | 80.5 |
| Toucan (lb) | lb, zero-shot | 3.498 | **0.832** | 0.224 | 79.8 |
| *LuxEmo-adapted systems* | | | | | |
| Qwen3\_FT | lb, fine-tuned | 3.357 | 13.263 | 0.315 | 133.0 |
| kNN TTS | lb, kNN prosody | 0.920 | 1.807 | 0.114 | 64.2 |

### Cross-lingual comparison (Table 2 in paper)

| Metric | XTTS (de) | Toucan (lb) | Δ (lb−de) | Better |
|:-------|:---------:|:-----------:|:---------:|:------:|
| WV MOS | 3.515 | 3.498 | −0.017 | de |
| Whisper WER | 1.768 | 1.231 | −0.537 | **lb** |
| LuxASR WER | 1.107 | 0.832 | −0.275 | **lb** |
| Speaker Sim | 0.317 | 0.224 | −0.093 | de |
| F0 RMSE | 80.5 | 79.8 | −0.7 | **lb** |

---

## Subjective Evaluation Results (Section 4.3)

Ten native Luxembourgish listeners (ages 20–50, balanced gender, self-reported normal hearing) each evaluated 20 stimuli (5 systems × 4 emotions) in 12–15 minute sessions, yielding 600 ratings total.

### Naturalness and emotion match (5-point MOS)

| Model | Naturalness | Emotion match |
|:------|:-----------:|:-------------:|
| Qwen3\_FT (lb) | **3.9** | **4.0** |
| Toucan (lb) | 3.7 | 3.8 |
| GradTTS (de) | 3.7 | 3.6 |
| XTTS (de) | 3.4 | 3.4 |
| kNN TTS (lb) | 2.3 | 2.4 |

### Emotion recognition accuracy (pooled across systems)

| Emotion | Accuracy |
|:--------|:--------:|
| Happy | ~80% |
| Neutral | ~75% |
| Sad | ~65% |
| Angry | ~55% |

### Inter-rater agreement (Krippendorff's α)

| Dimension | α |
|:----------|:-:|
| Naturalness | 0.60 |
| Emotion match | 0.56 |
| Intensity | 0.48 |

---

## LuxEmo Corpus Statistics (Table 1 in paper)

| Spk | Gender | Segments | Duration (min) | Neutral | Happy | Sad | Angry |
|:---:|:------:|:--------:|:--------------:|:-------:|:-----:|:---:|:-----:|
| 1 | M | 1,240 | 206.7 | 88 | 1,125 | 17 | 10 |
| 2 | F | 766 | 127.7 | 190 | 476 | 100 | 0 |
| 3 | F | 3,577 | 596.2 | 1,627 | 1,223 | 702 | 25 |
| 4 | F | 1,979 | 329.8 | 1,063 | 836 | 77 | 3 |
| **Total** | **1M, 3F** | **7,562** | **1,260.4** | **2,968** | **3,660** | **896** | **38** |

Corpus-level comparison: EmoDB (de, 0.4h, 10 speakers, 7 emotions, acted, studio) vs. **LuxEmo** (lb+code-switching, **21.0h**, 4 speakers, 4 emotions, **spontaneous**, youth media).
