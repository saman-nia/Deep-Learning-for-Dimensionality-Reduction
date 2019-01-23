# Deep Learning for Dense Matrix (e.g Wine Dataset) Dimensionality Reduction

Esay run:<br />
Use google colab to run the code. No need dependencies on the Google Colab. <br />
To run the code on google colab, go to the .ipynb files, then click on "Open in Colab" on the button above.<br />

We worked out on an idea based on providing a method to manage the new arrival sample into autoencoder. We kept a few samples for the test set, then we trained the model with the train set. After learning, we computed cosine distance between a new sample and each individual training set, then we found the index of the nearest sample in the training set to the new sample, then we replaced it on the training set, after that we computed graph similarity for the new training set. We passed this new graph similarity through the learned autoencoder.<br />

Performance of Autoencoder (AE) on the Wine Dataset:<br />

![Alt text](https://github.com/saman-nia/Deep-Learning-for-Dense-Matrix-Dimensionality-Reduction/blob/master/Dense%20Matrix%20Embedded/Autoencoder%20Performance.png?raw=true "Title")

Performance of different techniques of dimensionality reduction on the Wine Dataset:<br />

![Alt text](https://github.com/saman-nia/Deep-Learning-for-Dense-Matrix-Dimensionality-Reduction/blob/master/Dense%20Matrix%20Embedded/Comparison%20of%20techniques.png?raw=true "Title")

Performance of KMeans on different techniques of dimensionality reduction on the Wine Dataset:<br />

![Alt text](https://github.com/saman-nia/Deep-Learning-for-Dense-Matrix-Dimensionality-Reduction/blob/master/Dense%20Matrix%20Embedded/Comparison%20of%20techniques%20KMeans.png?raw=true "Title")


# Dependencies:
Python (>= 3.4) <br />
NumPy (>= 1.8.2) <br />
SciPy (>= 0.13.3) <br />
scikit-learn (>= 0.20) <br />
TensorFlow (>= 1.2) <br />
