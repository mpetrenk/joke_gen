# joke_generation
Training a joke generator with bidirectional LSTM

 ## Overview
 The goal was to train a model to predict the punchlines of canned jokes. The method was defined and applied in poetry generation projects
 
## Dataset: 
 https://www.kaggle.com/abhinavmoudgil95/short-jokes

The entire dataset contains ~230,000 jokes. Building the the bidirectional LSTM model resulted in roughly 27M parameters, which was too computationally costly for any configuration tried. The notebooks target the subset of 2000 (executed on a local Jupyter notebook) and 20000 (trained on a spark cluster) jokes

The code was adapted from the following Colab project on predicting Irish poetry 
https://colab.research.google.com/github/lmoroney/dlaicourse/blob/master/TensorFlow%20In%20Practice/Course%203%20-%20NLP/Course%203%20-%20Week%204%20-%20Lesson%202%20-%20Notebook.ipynb

