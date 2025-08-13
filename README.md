# Neural Chatbot

A sequence-to-sequence (Seq2Seq) chatbot with attention, trained on the Cornell Movie-Dialogs Corpus. Supports both training and interactive chat modes.

## Features

* **Seq2Seq with Attention:** Built using TensorFlow's legacy `embedding_attention_seq2seq`.
* **Bucketing & Padding:** Handles variable-length conversations efficiently.
* **Greedy Decoding:** Generates real-time responses.
* **Data Preprocessing:** Tokenization, vocabulary building, and ID mapping.
* **Modes:** Train from scratch or chat with a trained model.

## Dataset

* [Cornell Movie-Dialogs Corpus](https://www.cs.cornell.edu/~cristian/Cornell_Movie-Dialogs_Corpus.html)
  Place the extracted folder inside `data/` and set `DATA_PATH` in `config.py`.

## Requirements

* Python 3.x
* TensorFlow 1.x
* NumPy

Install dependencies:

```bash
pip install tensorflow==1.15 numpy
```

## Usage

Preprocess data, train, and chat:

```bash
# Train the chatbot
python main.py --mode train

# Chat with the bot
python main.py --mode chat
```


