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

Representative synthesized samples for each system and target emotion. Samples are from the four LuxEmo speakers (Spk1: M, Spk2–4: F). For the subjective evaluation, listeners assessed each sample on three dimensions:

1. **Perceived emotion** — Neutral / Happy / Sad / Angry / Other
2. **Emotion intensity** — 1 (none) to 5 (very strong)
3. **Naturalness & appropriateness** — 1 (poor) to 5 (excellent)

### Neutral

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| Spk1 (M) | [listen](Samples/GradTTS/neutral/Spk1_neutral_000.wav) | [listen](Samples/XTTS/neutral/Spk1_neutral_000.wav) | [listen](Samples/Toucan/neutral/Spk1_neutral_000.wav) | [listen](Samples/Qwen3_FT/neutral/Spk1_neutral_000.wav) | [listen](Samples/kNN_TTS/neutral/Spk1_neutral_000.wav) |
| Spk2 (F) | [listen](Samples/GradTTS/neutral/Spk2_neutral_000.wav) | [listen](Samples/XTTS/neutral/Spk2_neutral_000.wav) | [listen](Samples/Toucan/neutral/Spk2_neutral_000.wav) | [listen](Samples/Qwen3_FT/neutral/Spk2_neutral_000.wav) | [listen](Samples/kNN_TTS/neutral/Spk2_neutral_000.wav) |
| Spk3 (F) | [listen](Samples/GradTTS/neutral/Spk3_neutral_000.wav) | [listen](Samples/XTTS/neutral/Spk3_neutral_000.wav) | [listen](Samples/Toucan/neutral/Spk3_neutral_000.wav) | [listen](Samples/Qwen3_FT/neutral/Spk3_neutral_000.wav) | [listen](Samples/kNN_TTS/neutral/Spk3_neutral_000.wav) |
| Spk4 (F) | [listen](Samples/GradTTS/neutral/Spk4_neutral_000.wav) | [listen](Samples/XTTS/neutral/Spk4_neutral_000.wav) | [listen](Samples/Toucan/neutral/Spk4_neutral_000.wav) | [listen](Samples/Qwen3_FT/neutral/Spk4_neutral_000.wav) | [listen](Samples/kNN_TTS/neutral/Spk4_neutral_000.wav) |

### Happy

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| Spk1 (M) | [listen](Samples/GradTTS/happy/Spk1_happy_000.wav) | [listen](Samples/XTTS/happy/Spk1_happy_000.wav) | [listen](Samples/Toucan/happy/Spk1_happy_000.wav) | [listen](Samples/Qwen3_FT/happy/Spk1_happy_000.wav) | [listen](Samples/kNN_TTS/happy/Spk1_happy_000.wav) |
| Spk2 (F) | [listen](Samples/GradTTS/happy/Spk2_happy_000.wav) | [listen](Samples/XTTS/happy/Spk2_happy_000.wav) | [listen](Samples/Toucan/happy/Spk2_happy_000.wav) | [listen](Samples/Qwen3_FT/happy/Spk2_happy_000.wav) | [listen](Samples/kNN_TTS/happy/Spk2_happy_000.wav) |
| Spk3 (F) | [listen](Samples/GradTTS/happy/Spk3_happy_000.wav) | [listen](Samples/XTTS/happy/Spk3_happy_000.wav) | [listen](Samples/Toucan/happy/Spk3_happy_000.wav) | [listen](Samples/Qwen3_FT/happy/Spk3_happy_000.wav) | [listen](Samples/kNN_TTS/happy/Spk3_happy_000.wav) |
| Spk4 (F) | [listen](Samples/GradTTS/happy/Spk4_happy_000.wav) | [listen](Samples/XTTS/happy/Spk4_happy_000.wav) | [listen](Samples/Toucan/happy/Spk4_happy_000.wav) | [listen](Samples/Qwen3_FT/happy/Spk4_happy_000.wav) | [listen](Samples/kNN_TTS/happy/Spk4_happy_000.wav) |

### Sad

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| Spk1 (M) | [listen](Samples/GradTTS/sad/Spk1_sad_000.wav) | [listen](Samples/XTTS/sad/Spk1_sad_000.wav) | [listen](Samples/Toucan/sad/Spk1_sad_000.wav) | — | [listen](Samples/kNN_TTS/sad/Spk1_sad_000.wav) |
| Spk2 (F) | [listen](Samples/GradTTS/sad/Spk2_sad_000.wav) | [listen](Samples/XTTS/sad/Spk2_sad_000.wav) | [listen](Samples/Toucan/sad/Spk2_sad_000.wav) | — | [listen](Samples/kNN_TTS/sad/Spk2_sad_000.wav) |
| Spk3 (F) | [listen](Samples/GradTTS/sad/Spk3_sad_000.wav) | [listen](Samples/XTTS/sad/Spk3_sad_000.wav) | [listen](Samples/Toucan/sad/Spk3_sad_000.wav) | — | [listen](Samples/kNN_TTS/sad/Spk3_sad_000.wav) |
| Spk4 (F) | [listen](Samples/GradTTS/sad/Spk4_sad_000.wav) | [listen](Samples/XTTS/sad/Spk4_sad_000.wav) | [listen](Samples/Toucan/sad/Spk4_sad_000.wav) | — | [listen](Samples/kNN_TTS/sad/Spk4_sad_000.wav) |

### Angry

Anger is the rarest emotion in LuxEmo (0.5% of segments, 38 total). Samples from Spk2 and Spk3.

| | GradTTS (de) | XTTS (de) | Toucan (lb) | Qwen3\_FT (lb) | kNN TTS (lb) |
|:---|:---:|:---:|:---:|:---:|:---:|
| Spk2 (F) | [listen](Samples/GradTTS/angry/Spk2_angry_000.wav) | [listen](Samples/XTTS/angry/Spk2_angry_000.wav) | [listen](Samples/Toucan/angry/Spk2_angry_000.wav) | — | [listen](Samples/kNN_TTS/angry/Spk2_angry_000.wav) |
| Spk3 (F) | [listen](Samples/GradTTS/angry/Spk3_angry_000.wav) | [listen](Samples/XTTS/angry/Spk3_angry_000.wav) | [listen](Samples/Toucan/angry/Spk3_angry_000.wav) | — | [listen](Samples/kNN_TTS/angry/Spk3_angry_000.wav) |

Qwen3\_FT was fine-tuned with prompt-based emotion control for neutral and happy conditions; sad and angry synthesis was not available for this model.


