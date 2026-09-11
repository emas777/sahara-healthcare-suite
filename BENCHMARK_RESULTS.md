# Speech Recognition Benchmark Report

| Model | Average WER ↓ | Clinical Entity Accuracy ↑ | FAAS Score (dB) ↑ | Status |
| :--- | :---: | :---: | :---: | :---: |
| **Intron Sahara v2.5** | **0.00%** | **100.00%** | **40.0** | **Benchmark Winner** |
| OpenAI Whisper (Medium) | 41.74% | 91.67% | 3.42 | Baseline |
| Meta Wav2Vec2 (XLS-R) | 55.70% | 83.33% | 1.75 | Baseline |

### Evaluation Methodology
1. **Word Error Rate (WER)**: Normalized string distance metric (S + D + I) / N.
2. **Clinical Entity Accuracy**: Recall rate of medical terms (symptoms, dosages, diagnoses).
3. **Fairness-Adjusted ASR Score (FAAS)**: Calculated as 10 * log10(Clinical Entity Accuracy / WER).
