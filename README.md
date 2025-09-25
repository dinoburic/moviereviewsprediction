# Movie Review Sentiment Analysis

This repository contains a **machine learning model** that predicts whether an IMDb movie review is **positive** or **negative**, along with a **Gradio web app** to interact with the model in real time.

The model was trained on the **IMDb movie reviews dataset**.

You can try the live app here: [Review Sentiment App](https://huggingface.co/spaces/dinoburic/moviereviewsprediction)

---

## Files in this repository

- `app.py` – the main Gradio web app code.
- `IMDbModel.h5` – trained Keras sentiment analysis model.
- `tokenizer.pkl` – tokenizer used for preprocessing text.
- `requirements.txt` – required Python packages for running the app.

---

## How it works

1. The model takes a movie review as input.
2. The review is tokenized and padded to a fixed length.
3. The Keras model predicts the sentiment:
   - `positive` if the score > 0.5
   - `negative` otherwise
4. Gradio displays the result in a simple web interface.

---

## Running Locally

1. Clone this repository:

```bash
git clone https://github.com/dinoburic/moviereviewsprediction.git
cd moviereviewsprediction
