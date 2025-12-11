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

1.  **Clone the repository.**
2.  **Install dependencies** using the `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```
3.  **Open the `3rd period final.ipynb` file** in Google Colab and run all cells.
## ⚠️ Note on Notebook Display
The notebook (`3rd period final.ipynb`) may display an "Invalid Notebook" error when viewed directly on GitHub due to metadata from Google Colab widgets.
**Please click the 'Open in Colab' badge (if available) or download the file and upload it to Google Colab to view and run the code correctly.** The code itself is intact.
