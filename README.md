# Handwritten_digits_classification

  Handwritten digit classification is a classic machine learning project that uses the MNIST dataset, which contains images of handwritten digits from 0 to 9. The goal is to train a model to accurately classify the digits based on their pixel values.

**Dataset**
-->MNIST Dataset
A dataset of 70,000 grayscale images of handwritten digits.
Image Size: 28x28 pixels (flattened into 784 features for each image).
Classes: 10 (digits 0 through 9).
Train-Test Split:
60,000 training images.
10,000 testing images.

**Methadology**
1. Loading the Dataset.
2. Data Normalization: Scaling pixel values between 0 and 1 improves training stability.
3. Data Flattening: Flattening data from 2-D array to single Dimensional Array.
4. Building a Model:
5. 1. Model is trained with only a input layer with 10 Neurons and "Sigmoid" is a activation function. Then the model is tested for a flattened test data with 10 epoches.
   2. Model is trained along with the input layer with 100 neuron and "relu" activation function one hidden layer is added with 10 neurons and "Sigmoid" activation function to improve accuracy. Then the model is tested for flattened test data with 5 epoches.
   3. The model is trained with a scaled data(not flattened) by adding the flatten layer to the same model trained in 2nd run. This helps to improve the accuracy.
6. All the above models are compiled with "adam" optimizer and 'sparse_categorical_crossentropy' loss.
7. To compare the results of the above models confusion matrix is plotted.
