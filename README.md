# Automatic Text Summarizer Project

## Abstract

The project aims to develop an automatic text summarizer to assist researchers, journalists, and other users in quickly obtaining key information from large volumes of text. The goal is to create summaries comparable in quality to those written by humans. This involves designing a deep learning-based abstractive summarizer using a Seq2Seq architecture with multiple layers of LSTMs for both the Encoder and Decoder. The model incorporates Bahadnau Attention mechanism, allowing it to focus on specific parts of the input text while generating summaries.

## Implementation

The project successfully developed a deep learning model for automatic text summarization, including a user interface for easy interaction.

### Approach

1. **Word Embeddings:**
   - Extract embeddings for words using approaches like Word2Vec, GloVe, or Google's BERT.
2. **LSTM Processing:**
   - Use LSTMs for processing sequences of inputs.
3. **Seq2Seq Model:**
   - Build a Seq2Seq model with an encoder creating a fixed-size representation of the input sequence and a decoder predicting a sequence.
4. **Attention Mechanism:**
   - Implement attention between the encoder and decoder to focus on specific words rather than the entire sentence.
5. **Beam Search:**
   - Utilize beam search for more efficient predictions.

## Data-set

- Earlier dataset used was CNN/DailyMail
- Shifted to Amazon Fine Food Reviews dataset due to computational constraints
- Review lengths mostly within 60 words on average
- Summary lengths range from 2-8 words

## Implementation

- Extracted embeddings for each review
- Created one-hot vector for the summary
- Built encoder and decoder network with one LSTM layer
- Padded review and summary lengths to a fixed size
- Trained the model for 10k stories
- Ran for 20 epochs

## Conclusions

The project successfully implemented a LSTM model for Abstractive Text Summarization, providing concise summaries of food reviews. 
The model captures sentiments and identifies the main product mentioned in the reviews. 
A user-friendly interface was developed, enabling users to input sentences for summary generation. 
The effectiveness of the model can be best evaluated with food reviews, given the chosen dataset's domain.
