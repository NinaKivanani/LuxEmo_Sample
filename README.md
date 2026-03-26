# LuxEmo: Expressive Text-to-Speech Corpus for Luxembourgish

**Synthesized Audio Samples — Interspeech 2026**

---

LuxEmo comprises **21.0 hours** of wideband speech (7,562 ten-second segments) from four speakers annotated for four emotions in a code-switching Luxembourgish setting. We benchmark five expressive TTS systems. This page provides representative synthesized samples for side-by-side listening.

---

## Systems

| Model | Type | Language | Emotion Control |
|:------|:-----|:---------|:----------------|
| **GradTTS** | Diffusion | de (zero-shot) | Reference audio |
| **XTTS** | Cross-lingual | de (zero-shot) | Reference audio |
| **Toucan** | Reference encoder | lb (multilingual) | Reference vector |
| **Qwen3\_FT** | LLM-native fine-tuned | lb (adapted) | Prompt |
| **kNN TTS** | GlowTTS + SSL | lb (adapted) | kNN prosody retrieval |

---

## Listening Instructions

For each sample, please assess:

1. **Perceived emotion** — Which emotion do you hear? *(Neutral / Happy / Sad / Angry / Other)*
2. **Emotion intensity** — How strong is it? *(1 = None, 2 = Slight, 3 = Moderate, 4 = Strong, 5 = Very strong)*
3. **Naturalness and appropriateness** — How natural and emotionally appropriate does it sound? *(1–5)*

---

## Neutral

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| **Spk1** (M) | [wav](Samples/GradTTS/neutral/Spk1_neutral_000.wav) | [wav](Samples/XTTS/neutral/Spk1_neutral_000.wav) | [wav](Samples/Toucan/neutral/Spk1_neutral_000.wav) | [wav](Samples/Qwen3_FT/neutral/Spk1_neutral_000.wav) | [wav](Samples/kNN_TTS/neutral/Spk1_neutral_000.wav) |
| **Spk2** (F) | [wav](Samples/GradTTS/neutral/Spk2_neutral_000.wav) | [wav](Samples/XTTS/neutral/Spk2_neutral_000.wav) | [wav](Samples/Toucan/neutral/Spk2_neutral_000.wav) | [wav](Samples/Qwen3_FT/neutral/Spk2_neutral_000.wav) | [wav](Samples/kNN_TTS/neutral/Spk2_neutral_000.wav) |
| **Spk3** (F) | [wav](Samples/GradTTS/neutral/Spk3_neutral_000.wav) | [wav](Samples/XTTS/neutral/Spk3_neutral_000.wav) | [wav](Samples/Toucan/neutral/Spk3_neutral_000.wav) | [wav](Samples/Qwen3_FT/neutral/Spk3_neutral_000.wav) | [wav](Samples/kNN_TTS/neutral/Spk3_neutral_000.wav) |
| **Spk4** (F) | [wav](Samples/GradTTS/neutral/Spk4_neutral_000.wav) | [wav](Samples/XTTS/neutral/Spk4_neutral_000.wav) | [wav](Samples/Toucan/neutral/Spk4_neutral_000.wav) | [wav](Samples/Qwen3_FT/neutral/Spk4_neutral_000.wav) | [wav](Samples/kNN_TTS/neutral/Spk4_neutral_000.wav) |

## Happy

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| **Spk1** (M) | [wav](Samples/GradTTS/happy/Spk1_happy_000.wav) | [wav](Samples/XTTS/happy/Spk1_happy_000.wav) | [wav](Samples/Toucan/happy/Spk1_happy_000.wav) | [wav](Samples/Qwen3_FT/happy/Spk1_happy_000.wav) | [wav](Samples/kNN_TTS/happy/Spk1_happy_000.wav) |
| **Spk2** (F) | [wav](Samples/GradTTS/happy/Spk2_happy_000.wav) | [wav](Samples/XTTS/happy/Spk2_happy_000.wav) | [wav](Samples/Toucan/happy/Spk2_happy_000.wav) | [wav](Samples/Qwen3_FT/happy/Spk2_happy_000.wav) | [wav](Samples/kNN_TTS/happy/Spk2_happy_000.wav) |
| **Spk3** (F) | [wav](Samples/GradTTS/happy/Spk3_happy_000.wav) | [wav](Samples/XTTS/happy/Spk3_happy_000.wav) | [wav](Samples/Toucan/happy/Spk3_happy_000.wav) | [wav](Samples/Qwen3_FT/happy/Spk3_happy_000.wav) | [wav](Samples/kNN_TTS/happy/Spk3_happy_000.wav) |
| **Spk4** (F) | [wav](Samples/GradTTS/happy/Spk4_happy_000.wav) | [wav](Samples/XTTS/happy/Spk4_happy_000.wav) | [wav](Samples/Toucan/happy/Spk4_happy_000.wav) | [wav](Samples/Qwen3_FT/happy/Spk4_happy_000.wav) | [wav](Samples/kNN_TTS/happy/Spk4_happy_000.wav) |

## Sad

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| **Spk1** (M) | [wav](Samples/GradTTS/sad/Spk1_sad_000.wav) | [wav](Samples/XTTS/sad/Spk1_sad_000.wav) | [wav](Samples/Toucan/sad/Spk1_sad_000.wav) | — | [wav](Samples/kNN_TTS/sad/Spk1_sad_000.wav) |
| **Spk2** (F) | [wav](Samples/GradTTS/sad/Spk2_sad_000.wav) | [wav](Samples/XTTS/sad/Spk2_sad_000.wav) | [wav](Samples/Toucan/sad/Spk2_sad_000.wav) | — | [wav](Samples/kNN_TTS/sad/Spk2_sad_000.wav) |
| **Spk3** (F) | [wav](Samples/GradTTS/sad/Spk3_sad_000.wav) | [wav](Samples/XTTS/sad/Spk3_sad_000.wav) | [wav](Samples/Toucan/sad/Spk3_sad_000.wav) | — | [wav](Samples/kNN_TTS/sad/Spk3_sad_000.wav) |
| **Spk4** (F) | [wav](Samples/GradTTS/sad/Spk4_sad_000.wav) | [wav](Samples/XTTS/sad/Spk4_sad_000.wav) | [wav](Samples/Toucan/sad/Spk4_sad_000.wav) | — | [wav](Samples/kNN_TTS/sad/Spk4_sad_000.wav) |

## Angry

> Anger is the rarest emotion in LuxEmo (0.5% of segments). Samples from two speakers.

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| **Spk2** (F) | [wav](Samples/GradTTS/angry/Spk2_angry_000.wav) | [wav](Samples/XTTS/angry/Spk2_angry_000.wav) | [wav](Samples/Toucan/angry/Spk2_angry_000.wav) | — | [wav](Samples/kNN_TTS/angry/Spk2_angry_000.wav) |
| **Spk3** (F) | [wav](Samples/GradTTS/angry/Spk3_angry_000.wav) | [wav](Samples/XTTS/angry/Spk3_angry_000.wav) | [wav](Samples/Toucan/angry/Spk3_angry_000.wav) | — | [wav](Samples/kNN_TTS/angry/Spk3_angry_000.wav) |

---

## Results

### Cross-lingual comparison (Table 2 in paper)

| Metric | XTTS (de) | Toucan (lb) | Better |
|:-------|:---------:|:-----------:|:------:|
| WV MOS | 3.515 | 3.498 | de |
| Whisper WER | 1.768 | 1.231 | **lb** |
| LuxASR WER | 1.107 | 0.832 | **lb** |
| Speaker Sim | 0.317 | 0.224 | de |
| F0 RMSE | 80.5 | 79.8 | **lb** |

### Subjective evaluation (10 native Luxembourgish listeners)

| Model | Naturalness (MOS) | Emotion match (MOS) |
|:------|:-----------------:|:-------------------:|
| Qwen3\_FT (lb) | **3.9** | **4.0** |
| Toucan (lb) | 3.7 | 3.8 |
| GradTTS (de) | 3.7 | 3.6 |
| XTTS (de) | 3.4 | 3.4 |
| kNN TTS (lb) | 2.3 | 2.4 |

### Emotion recognition accuracy (pooled)

| Emotion | Accuracy |
|:--------|:--------:|
| Happy | ~80% |
| Neutral | ~75% |
| Sad | ~65% |
| Angry | ~55% |

Inter-rater agreement: naturalness alpha = 0.60, emotion match alpha = 0.56, intensity alpha = 0.48.

---

## Corpus

| Spk | G | Segs | Min | N | H | S | A |
|:---:|:-:|:----:|:---:|:---:|:---:|:---:|:---:|
| 1 | M | 1,240 | 206.7 | 88 | 1,125 | 17 | 10 |
| 2 | F | 766 | 127.7 | 190 | 476 | 100 | 0 |
| 3 | F | 3,577 | 596.2 | 1,627 | 1,223 | 702 | 25 |
| 4 | F | 1,979 | 329.8 | 1,063 | 836 | 77 | 3 |
| **All** | **1M,3F** | **7,562** | **1,260.4** | **2,968** | **3,660** | **896** | **38** |

