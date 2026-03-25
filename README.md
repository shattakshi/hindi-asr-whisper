# Hindi ASR using Whisper

This project implements an end-to-end Automatic Speech Recognition (ASR) pipeline for Hindi conversational speech using OpenAI Whisper models.

---

## 📌 Overview

The system processes raw audio data and generates transcriptions using Whisper, followed by evaluation and post-processing to improve output quality.

---

## ⚙️ Features

- Data downloading and preprocessing
- Audio segmentation using timestamps
- Whisper-based transcription (small & medium models)
- Word Error Rate (WER) evaluation
- Post-processing pipeline for improving text quality
- Word-level classification (correct vs incorrect)

---

## 📂 Project Structure


hindi-asr-whisper/
│
├── src/
│ ├── load_data.py
│ ├── inspect_data.py
│ ├── download_data.py
│ ├── segment_audio.py
│ ├── build_dataset.py
│ ├── run_whisper.py
│ ├── evaluate.py
│ ├── postprocess_full.py
│ └── word_classifier.py
│
├── data/
│ ├── raw/
│ ├── processed/
│ └── word_list.txt
│
└── README.md


---

## 🚀 Pipeline

1. **Data Preparation**
   - Download audio and transcription files
   - Clean and structure dataset

2. **Audio Segmentation**
   - Split long recordings into smaller segments

3. **Model Inference**
   - Use Whisper models for transcription

4. **Evaluation**
   - Compute Word Error Rate (WER)

5. **Post-processing**
   - Remove repetition
   - Normalize text

6. **Word Classification**
   - Identify correct and incorrect words using rules

---

## 📊 Results

| Model | WER |
|------|------|
| Whisper Small | 0.83 |
| Improved Whisper (Medium) | 0.47 |

---

## 🔍 Error Analysis

Common issues observed:
- Repetition errors
- Word merging
- Phonetic inaccuracies
- Conversational noise impact

---

## 🛠️ Improvements

- Used larger Whisper model for better accuracy
- Implemented post-processing pipeline
- Added word-level validation

---

## 📌 Conclusion

This project demonstrates a complete Hindi ASR workflow, highlighting challenges in conversational speech recognition and practical approaches to improving transcription quality.

---

## 👤 Author

Shatakshi Tiwari
