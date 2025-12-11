# Emotion-Text-Classifier-HuggingFace
Fine-tuning DistilBERT for emotion classification using the dair-ai/emotion dataset.
# Emotion-Text-Classifier-HuggingFace

Fine-tuning DistilBERT for emotion classification using the dair-ai/emotion dataset.

## 🎯 Project Goals

This project implements a text classification system using the Hugging Face Transformers library to classify social media text into six core emotions (joy, sadness, anger, fear, love, surprise).

## 📊 Dataset and Model

* **Dataset:** [dair-ai/emotion](https://huggingface.co/datasets/dair-ai/emotion) (200 training examples and 50 test examples were sampled for fast fine-tuning).
* **Model:** [distilbert-base-uncased-emotion](https://huggingface.co/bhadresh-savani/distilbert-base-uncased-emotion)
* **Technique:** Transfer Learning via Fine-tuning.

## 📝 Deliverables

The following files are included in this repository:
* `3rd period final.ipynb`: The complete Google Colab notebook containing all code, EDA, training, and evaluation steps.
* `Project_Report.pdf`: A detailed report/presentation summarizing the project implementation and results.
* `requirements.txt`: A list of required Python packages to run the notebook.

## ⭐ Key Results

After fine-tuning for one epoch:
* **Overall Accuracy (Test Set):** 42%
* **Observation:** The low accuracy is expected due to the highly limited training sample size (200 examples) and class imbalance.
* **Key Performance:** The model showed very high performance on the dominant class, **Joy** (100% Recall), but failed to classify rare classes like Love and Fear (0% F1-score), highlighting the effect of data sparsity.

## 🚀 How to Run the Project

### ⚠️ Important Note on Code Access ⚠️

The notebook (`3rd period final.ipynb`) cannot be displayed directly on GitHub due to internal metadata conflicts from Google Colab.

**To run the code:**

1.  **Click the 'Open in Colab' badge (if available)** which may appear on the file page.
2.  **OR, download the file** (`3rd period final.ipynb`) and upload it manually to Google Colab.

The code is complete and functional, but must be run within the Colab environment.

---

1.  **Install dependencies** using the `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```
2.  **Open the `3rd period final.ipynb` file** in Google Colab and run all cells.
