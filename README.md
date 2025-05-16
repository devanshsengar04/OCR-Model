# Handwriting OCR using TrOCR

This project fine-tunes Microsoft's TrOCR-base model to recognize handwritten text using the IAM dataset. The implementation was done entirely in a single Jupyter notebook in Google Colab.

## 📌 Objective

To build an OCR pipeline that mimics document digitization using a Transformer-based model and evaluate its accuracy on real handwriting samples.

## 🧠 Model

- **Model used**: `microsoft/trocr-base-handwritten`
- Fine-tuned on IAM dataset
- Achieved:
  - **Character Error Rate (CER)**: 4.77%
  - **Word Error Rate (WER)**: 11.55%

## 🗂 Dataset

- IAM Handwriting Dataset
- Preprocessed using `TrOCRProcessor` from Hugging Face

## 📊 Evaluation

- Used `evaluate` and `jiwer` libraries to compute CER and WER
- Verified model prediction on both test set and custom handwritten image

## 📝 Files

- `Devansh_Sengar_OCR_code.ipynb`: Complete notebook with training, evaluation, and inference
- `Devansh_sengar_OCR_Report.pdf`: Summarized project report

## 📌 Requirements

Install these before running:
```bash
pip install transformers datasets evaluate jiwer
