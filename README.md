# Cinemania: Movie Sentiment Analysis (RNN vs. Transformer)

This project is an end-to-end sentiment analysis system developed for
"Cinemania," a streaming service. The goal is to automatically classify
user movie reviews as either **Positive** or **Negative** by comparing
two different deep learning architectures.

## 🚀 Project Overview

In this project, I implemented and compared two distinct approaches to
Natural Language Processing (NLP): 1. **Recurrent Neural Network
(RNN):** A custom-built model using PyTorch, featuring a manually
constructed vocabulary (4000 words) and word embeddings. 2.
**Transformer (DistilBERT):** A state-of-the-art model leveraging
transfer learning from the Hugging Face `transformers` library.

## 📊 Key Features

-   **Data Preprocessing:** Handled text cleaning, tokenization, and
    padding for both models.
-   **Custom Vocabulary:** Built a word-to-index mapping from scratch
    for the RNN.
-   **Transfer Learning:** Fine-tuned `distilbert-base-uncased` for
    sequence classification.
-   **Model Comparison:** Evaluated both models based on loss metrics
    and real-world predictions.
-   **Interactive UI:** Integrated a Gradio web interface for real-time
    sentiment testing.

## 🛠️ Tech Stack

-   **Language:** Python
-   **Frameworks:** PyTorch, Hugging Face (Transformers, Datasets)
-   **Libraries:** Pandas, NumPy, Scikit-learn, Gradio
-   **Architecture:** DistilBERT, Vanilla RNN

## 📈 Results & Findings

  -----------------------------------------------------------------------
  Model             Training Epochs   Best Eval Loss    Verdict
  ----------------- ----------------- ----------------- -----------------
  **RNN**           10                Higher            Struggled with
                                                        long-range
                                                        dependencies and
                                                        complex context.

  **Transformer**   3                 **0.4138**        Exceptionally
                                                        accurate,
                                                        especially with
                                                        context-heavy
                                                        reviews.
  -----------------------------------------------------------------------

> **Conclusion:** The Transformer model significantly outperformed the
> RNN, demonstrating the power of pre-trained attention mechanisms in
> understanding linguistic nuances like contrast and sarcasm.

## 💻 Installation & Usage

1.  **Clone the repository:**

    ``` bash
    git clone https://github.com/your-username/cinemania-sentiment-analysis.git
    ```

2.  **Install dependencies:**

    ``` bash
    pip install -r requirements.txt
    ```

3.  **Run the Notebook:** Open the `.ipynb` file in Jupyter or Google
    Colab to see the full training process and launch the Gradio
    interface.

📝 Example Predictions

Input: "The cast is wonderful, and the plot is also very interesting."
-\> Result: Positive ✅

Input: "The visual effects are good, but the story is weak." -\> Result:
Negative ✅

------------------------------------------------------------------------

### 2. requirements.txt

Create a file named `requirements.txt` and add the following lines:

    torch
    transformers
    pandas
    numpy
    gradio
    scikit-learn
