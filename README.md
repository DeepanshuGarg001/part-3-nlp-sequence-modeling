# Part 3: NLP and Sequence Modeling Mini Project

## Project Overview
This project involves building a basic NLP pipeline to classify customer support queries. It compares traditional text vectorization (TF-IDF) with sequence-based deep learning (LSTM).

## Dataset
- **Source:** Provided Synthetic Dataset (`customer_support_text_classification.csv`)
- **Focus:** Classifying support tickets into categories.

## Tasks Covered
1. **Dataset Understanding:** Analyzing record counts, class distribution, and text length metrics.
2. **Text Preprocessing:** Cleaning, tokenization, and sequence padding.
3. **Text Vectorization:** Comparing TF-IDF with Tokenizer-based sequences.
4. **Baseline Model:** Logistic Regression with TF-IDF.
5. **Sequence Model:** Building and explaining an LSTM-based architecture.

## Task 6: Attention and Transformer Reflection
### 1. Why RNNs struggle with long-term dependencies?
RNNs process sequences step-by-step. As the sequence length increases, the information from early steps becomes diluted due to the "vanishing gradient" problem. By the time the network reaches the end of a long sentence, it has effectively "forgotten" the beginning.

### 2. How LSTMs help with memory?
LSTMs (Long Short-Term Memory) introduce a "cell state" and "gates" (input, forget, and output gates). These gates allow the network to explicitly decide what information to keep, what to throw away, and what to pass on, effectively preserving long-term dependencies.

### 3. What attention solves in sequence-to-sequence tasks?
Attention allows the model to "look back" at all parts of the input sequence and assign different weights (importance) to different words when generating each part of the output. This solves the bottleneck problem where a single fixed-length vector had to represent the entire input.

### 4. Why transformers are important in modern NLP and Generative AI?
Transformers replace recurrence with "Self-Attention," allowing for parallel processing of the entire sequence at once. This makes them much faster to train and far more effective at capturing global dependencies, forming the foundation for modern models like BERT and GPT.
