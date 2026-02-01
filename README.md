# N-Gram Language Models

**NLP Prosit 1 — Ankora Interns**

Experiments with n-gram language models: domain adaptation for healthcare (AfriMed-QA), LLM fine-tuning for medical MCQ generation, and n-gram–based correction for Twi speech transcription.

## Structure

```
NLP Prosit 1/
├── LM Adaptation/                    # Domain adaptation for AfriMed-QA healthcare MCQs
│   ├── LLM approach/
│   │   ├── AfriMed-QA data preprocessing.ipynb   # Load & filter AfriMed-QA v2 (MCQ only)
│   │   ├── LM fine-tuning for healthcare MCQ.ipynb   # Fine-tune TinyLlama, SmolLM2
│   │   └── README.md
│   └── n-gram approach/
│       └── ngram_finetuning_final.ipynb   # Bigram/trigram interpolation, Laplace smoothing, perplexity
│
├── n-gram for low-resource/          # Notes & resources for low-resource modeling
│   └── README.md
│
└── n-gram downstream application/    # ASR post-processing for Twi (Akan)
    ├── clean_transcription_pipeline.ipynb   # Whisper transcription + n-gram correction (Common Voice)
    ├── cv-corpus-24.0-2025-12-05.rar
    └── twi audio.rar
```