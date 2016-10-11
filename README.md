# Short Text Categorization with Word Embeddings

This repository is a collection of algorithms for multi-class classification to short texts using Python. Instead of the bag-of-words representation of texts, word-embedding algorithms with a pre-trained model are used. Currently, Word2Vec is implemented.

So far the following algorithms are implemented:

* SumWord2Vec: each short text is represented by the average of the embedded vectors of all the words.
* Autoencoder: the embedded vectors are passed into an autoencoded representation, where the similarity is calculated by cosine.
* Convolutional Neural Network (CNN): all the words are represented by embedded vectors, which are passed into a convolional neural network.

The Word2Vec model is implemented with [`gensim`](https://radimrehurek.com/gensim/), and CNN with [`keras`](https://keras.io/), with a [`Theano`](http://deeplearning.net/software/theano/) backend.

# Further Reading

* Tomas Mikolov, Ilya Sutskever, Kai Chen, Greg Corrado, Jeffrey Dean, "Distributed Representations of Words and Phrases and their Compositionality", *NIPS Proceedings* __26__, 3111-3119 (2013). \[[arXiv](https://arxiv.org/abs/1310.4546)\]
* Yoon Kim, "Convolutional Neural Networks for Sentence Classification" (2014). \[[arXiv](https://arxiv.org/abs/1408.5882)\]

