# SensEmBERT

We are now busy with ACL deadline. A better interface will be 
provided right after the 10th of Dicember!

In the meanwhile, in this repository you can find the data for the paper: [SensEmBERT: Context-Enhanced Sense Embeddings for Multilingual Word Sense Disambiguation](https://pasinit.github.io/papers/scarlini_etal_aaai2020.pdf).

We made available two distinct set of vectors for all WordNet synsets:
- [sensembert_supervised.txt]() which contains 2348 dimensional vectors
with the first 1024 dimensions encoding the gloss and the large contextual
information gathered as described in the paper. The second 1024 encoding 
the information coming from SemCor and the last 300 encoding the word
information by means of fasttext vectors.
- [sensembert_kb.txt]() which contains 2348 dimensional vectors
with the first 1024 dimensions encoding the contextual information
gathered as described in the paper, the second 1024 encoding the 
definitional information coming from the glosses and the last 300 encoding
the word-level information by means of fasttext vectors.

Both files follow the word2vec format, i.e., a space-separated
file with the first column being the synset (bn:00000001n)
and the following 2348 numbers being the feature of the synset
vector.