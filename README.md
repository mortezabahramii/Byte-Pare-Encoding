# Byte-Pare-Encoding
This repo created for use Byte-Pare-Encoding(BPE) in NLP for tokenization.

One of the things do in NLP is tokenization and extracting words, which the Byte Pair Encoding (BPE) algorithm helps us in this work. In the article entitled "Neural Machine Translation of Rare Words with Subword Units" which was published in 2015, a piece of code for byte pair encoding was introduced. By checking different tokens and comparing the number of their repetitions, this algorithm can identify text tokens.

## Dataset
The dataset (TestText.txt) used is part of the English Wikipedia text about machine learning. It has been used to check and implement the algorithm.

## Implementation
The implementation of the BPE algorithm is such that all the text is received. It is processed line by line. At the beginning, a space character is placed between the letters of each word, and at the end, the </w> character is placed for separation. This character is used to separate words from each other and prevent two words from being combined together. Each letter is considered as a token and all of them are stored in a dictionary set. A new token is created by combining each token with other tokens. Based on the number of repetitions of new tokens, the token with the most repetition is considered as a new token. It repeats this task up to k times or continues when no token is combined with another token.

## Results
In 500 iterations, 320 tokens have been detected and some tokens are wrong. But in 1000 repetitions (the algorithm stopped at step 753), 260 tokens have been recognized as suitable and correct.
