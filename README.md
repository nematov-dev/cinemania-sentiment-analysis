# 🎬 Cinemania: Movie Sentiment Analysis (RNN vs Transformer)

An end-to-end Sentiment Analysis system built for **Cinemania**, a movie
streaming platform.\
The objective of this project is to automatically classify user movie
reviews as **Positive** or **Negative**, while comparing two different
deep learning architectures.

------------------------------------------------------------------------

## 🚀 Project Overview

This project implements and compares two NLP approaches:

### 1️⃣ Recurrent Neural Network (RNN)

-   Built from scratch using PyTorch
-   Custom vocabulary (4000 most frequent words)
-   Manual tokenization and padding
-   Word Embedding layer
-   Designed to understand sequential text data

### 2️⃣ Transformer (DistilBERT)

-   Pre-trained `distilbert-base-uncased`
-   Fine-tuned for sequence classification
-   Implemented using Hugging Face Transformers
-   Uses attention mechanisms for contextual understanding

------------------------------------------------------------------------

## 📊 Key Features

-   ✅ Text Cleaning & Preprocessing
-   ✅ Custom Vocabulary Construction
-   ✅ Word-to-Index Mapping
-   ✅ Manual Padding for RNN
-   ✅ Transfer Learning with DistilBERT
-   ✅ Model Evaluation & Comparison
-   ✅ Interactive Gradio Web Interface
-   ✅ Real-time Sentiment Prediction

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   **Language:** Python\
-   **Deep Learning:** PyTorch\
-   **NLP:** Hugging Face Transformers, Datasets\
-   **Data Processing:** Pandas, NumPy\
-   **Model Evaluation:** Scikit-learn\
-   **Web UI:** Gradio

------------------------------------------------------------------------

## 📈 Model Comparison

  -------------------------------------------------------------------------------
  Model          Training Epochs       Best Evaluation Loss       Performance
  -------------- --------------------- -------------------------- ---------------
  RNN            10                    Higher                     Struggled with
                                                                  long-range
                                                                  dependencies

  Transformer    3                     **0.4138**                 Excellent
  (DistilBERT)                                                    contextual
                                                                  understanding
  -------------------------------------------------------------------------------

------------------------------------------------------------------------

## 🧠 Key Findings

-   RNN models struggle with long-range dependencies and contextual
    nuances.
-   Transformer-based models significantly outperform traditional RNNs.
-   Pre-trained attention mechanisms dramatically improve performance.
-   DistilBERT handles contrastive sentences and sarcasm better.

> **Conclusion:** The Transformer model outperformed the RNN,
> demonstrating the effectiveness of transfer learning and
> attention-based architectures in sentiment analysis.

------------------------------------------------------------------------

## 📂 Project Structure

cinemania-sentiment-analysis/ │ ├── data/ ├── models/ ├── notebooks/ │
└── training_notebook.ipynb ├── app.py ├── requirements.txt └──
README.md

------------------------------------------------------------------------

## 💻 Installation & Setup

### 1️⃣ Clone the repository

git clone
https://github.com/your-username/cinemania-sentiment-analysis.git cd
cinemania-sentiment-analysis

### 2️⃣ Install dependencies

pip install -r requirements.txt

### 3️⃣ Run the Notebook

Open the `.ipynb` file in: - Jupyter Notebook - Google Colab - VS Code
Notebook environment

Train the models and launch the Gradio interface.

------------------------------------------------------------------------

## 🖥️ Running the Web App (If app.py is included)

python app.py

------------------------------------------------------------------------

## 📝 Example Predictions

**Input:**\
The cast is wonderful, and the plot is also very interesting.\
**Prediction:** Positive ✅

**Input:**\
The visual effects are good, but the story is weak.\
**Prediction:** Negative ✅

------------------------------------------------------------------------

## 🔮 Future Improvements

-   Add LSTM/GRU comparison
-   Add confusion matrix visualization
-   Deploy with Docker
-   Deploy on Hugging Face Spaces
-   Add multi-class sentiment support

------------------------------------------------------------------------

## 👨‍💻 Author

Developed by **Saidakbar Nematov**

------------------------------------------------------------------------

## 📜 License

This project is open-source and available under the MIT License.
