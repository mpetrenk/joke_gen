# joke_generation
Training a joke generator with bidirectional LSTM

 ## Overview
 The goal was to train a model to predict the punchlines of canned jokes. The method was defined and applied in poetry generation projects
 
## Dataset: 
 https://www.kaggle.com/abhinavmoudgil95/short-jokes

The entire dataset contains ~230,000 jokes. Building the the bidirectional LSTM model resulted in roughly 27M parameters, which was too computationally costly for any configuration tried. The notebooks target the subset of 2000 (executed on a local Jupyter notebook) and 20000 (trained on a spark cluster) jokes

## Code
The code was adapted from the following Colab project on predicting Irish poetry 
https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%204%20-%20Lesson%202%20-%20Notebook.ipynb

The notebook called joke_gen_pyspark is the non-distributed implementation of the same Keras model trained on a larger cluster. This allowed to use a larger dataset of 20000 jokes for training. With 70 epochs and over 3M parameters the achieved accuracy is mid 60's, and there was a steady increase in the accuracy at each epoch. I did not attempt to rerun the model due to limitations on the computing resources available. Depending on the available resources, it might be better to increase the number of epochs. 
