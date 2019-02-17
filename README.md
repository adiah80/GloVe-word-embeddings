# Glove-word-embeddings

This repo contains the implementation of the GloVe model for obtaining word embeddings.<br>
The original paper can be found a : https://nlp.stanford.edu/projects/glove/

* __Dataset__ : A random sample of 1000 reviews was chosen as the dataset to reduce the computational load. The sentences were tokenized and cleaned to remove stop words and then added to the corpus. The corpus was scanned to create a vocabulary and dictionaries that mapped words to indices and vice-versa.
* __Training__ : A co-orrurrence matrix was made from the corpus with a window size of 10 words both to the left and right of the centre word. Each word vector was initialised with a vector of dimension=15. The model was trained for 350 epochs and with a learning rate of 0.001 . The tsne vecotrs were generated and mapped on a 2D graph. A high-quality graph was saved to avoid pixelization when zooming in. Again, the complete neural network was implemented in numpy.
* __Loading__ : To load the model, run the appropriate marked-cell in the notebook. To load other small models, copy their respecitve .txt files into the main folder. The default files are for the 1000-review corpus training set with 350 iterations.
<br>
Reults : 

![](https://github.com/adiah80/glove-word-embeddings/blob/master/tsne%2C%20iter%3D350%2C%20dpi%3D100%2C%20words%3Dallby10.png)
