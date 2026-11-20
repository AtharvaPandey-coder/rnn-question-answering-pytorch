# Question Answering using a Simple RNN (PyTorch)

> **Note:** This is a learning project made only for practice, while following the CampusX deep learning course. It is not a production project.

## What it does
It reads a question and predicts the **first word** of the answer, using a simple RNN. If the model is not confident enough (probability below 0.5), it prints "I Don't know".

## Concepts practiced
- Text cleaning and tokenization
- Building a vocabulary from questions and answers
- Custom `Dataset` and `DataLoader` in PyTorch
- RNN model with an embedding layer
- Training loop with `CrossEntropyLoss` and Adam
- Softmax and a confidence threshold for predictions

## Tech used
Python, PyTorch, pandas

## Dataset
`100_Unique_QA_Dataset.csv` with two columns: `question` and `answer`. Keep it in the same folder as the code.

## How to run
```bash
pip install -r requirements.txt
python rnn_qa_model.py
```

## Limitations
- It predicts only the first word of the answer, not a full sentence.
- The dataset is small (100 rows), so it works best on questions similar to the training data.
- Practice project only.

## Future improvements
- Predict the full answer
- Add a Streamlit UI
