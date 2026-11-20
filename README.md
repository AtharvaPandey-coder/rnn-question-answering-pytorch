# Next Word Predictor using LSTM (PyTorch)

> **Note:** This is a learning project made only for practice, while following the CampusX deep learning course. It is not a production project.

## What it does
It reads a few words and predicts the next word, one word at a time, to generate text. It is trained on a small FAQ text (CampusX DSMP 2023 course FAQ), which is written inside the code.

## Concepts practiced
- Tokenization with NLTK
- Building a vocabulary (word to number)
- Creating training sequences and padding
- Custom `Dataset` and `DataLoader` in PyTorch
- LSTM model with an embedding layer
- Training loop (`zero_grad`, `backward`, `step`)
- Text generation using the trained model

## Tech used
Python, PyTorch, NLTK

## How to run
```bash
pip install -r requirements.txt
python next_word_lstm.py
```

## Example
Input: `the course follows`
The model then adds 10 predicted words, one by one.

## Limitations
- Trained on a very small text, so the generated sentences are only a demo and are not always meaningful.
- Practice project only.

## Future improvements
- Add a Streamlit UI
- Train on a larger dataset
