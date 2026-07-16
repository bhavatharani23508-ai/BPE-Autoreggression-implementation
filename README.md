# Custom Byte Pair Encoding (BPE) Tokenizer and Autoregressive Causal Language Model

## 📌 Project Overview

This project demonstrates a basic implementation of a **Byte Pair Encoding (BPE) Tokenizer** and a **Simplified Autoregressive Causal Language Model** using **Python** and **NumPy**.

The BPE tokenizer learns subword vocabulary by repeatedly merging the most frequent adjacent symbol pairs. The generated vocabulary is then used as the input for a simple autoregressive language model that predicts the next token in a sequence.

---

## 🎯 Objectives

- Build a Byte Pair Encoding (BPE) tokenizer from scratch.
- Learn merge rules from a text corpus.
- Generate a subword vocabulary.
- Encode and decode words using learned merge rules.
- Convert tokens into token IDs.
- Build a simple autoregressive language model.
- Demonstrate embeddings, positional encoding, causal masking, self-attention, softmax, cross-entropy loss, backpropagation, and next-token prediction.

---

## 🛠 Technologies Used

- Python 3
- NumPy
- Jupyter Notebook

---

## 📂 Project Structure

```
Project/
│
├── corpus.txt
├── BPE_Autoregressive.ipynb
└── README.md
```

---

## 📖 Corpus

Example corpus used for training:

```
low
lower
lowest
new
newer
widest
```

---

# Part 1 – Byte Pair Encoding (BPE)

## Implementation Steps

- Read the text corpus.
- Preprocess the text.
- Split each word into characters.
- Append the end-of-word symbol (`</w>`).
- Count word frequencies.
- Find adjacent symbol pairs.
- Count pair frequencies.
- Select the most frequent pair.
- Merge the pair.
- Update the vocabulary.
- Repeat until the required number of merges.
- Store merge rules.
- Build the final vocabulary.
- Implement encode().
- Implement decode().
- Test the tokenizer.

---

## BPE Output

The tokenizer generates:

- Initial Vocabulary
- Word Frequencies
- Merge Rules
- Final Vocabulary
- Vocabulary Size
- Encoded Tokens
- Decoded Text

---

# Part 2 – Autoregressive Causal Language Model

The output tokens from the BPE tokenizer are used as the input to a simplified autoregressive language model.

## Pipeline

```
Raw Text
      ↓
BPE Tokenizer
      ↓
Token IDs
      ↓
Input–Target Pairs
      ↓
Embedding
      ↓
Positional Encoding
      ↓
Causal Mask
      ↓
Self Attention
      ↓
Linear Layer
      ↓
Softmax
      ↓
Cross Entropy Loss
      ↓
Backpropagation
      ↓
Next Token Prediction
      ↓
Text Generation
```

---

## Features

- Token ID Mapping
- Input–Target Pair Creation
- Embedding Matrix
- Positional Encoding
- Causal Mask
- Self-Attention
- Linear Layer
- Softmax Activation
- Cross Entropy Loss
- Simplified Backpropagation
- Next Token Prediction
- Text Generation

---

## Sample Output

```
Token IDs:
[7, 2, 9]

Input:
[7, 2]

Target:
[2, 9]

Predicted Tokens:
['e', 'lower</w>']

Generated Text:
newestlowerlowerlower
```

**Note:** Since this is a simplified educational implementation with randomly initialized embeddings and weights, the generated text may not be meaningful. A fully trained autoregressive language model would produce meaningful predictions after training.

---

## Learning Outcomes

After completing this project, you will understand:

- Byte Pair Encoding (BPE)
- Subword Tokenization
- Vocabulary Learning
- Token IDs
- Embeddings
- Positional Encoding
- Causal Masking
- Self-Attention
- Softmax Function
- Cross Entropy Loss
- Backpropagation
- Next Token Prediction
- Text Generation

---
Python | NumPy | NLP | Byte Pair Encoding | Autoregressive Language Model
```
