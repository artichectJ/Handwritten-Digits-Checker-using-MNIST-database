# MNIST Handwritten Digit Recognition Using CNN
<img alt="Python" src="https://img.shields.io/badge/python-%2314354C.svg?style=for-the-badge&logo=python&logoColor=white"/> <img alt="NumPy" src="https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white" />  <img alt="Jupyter" src="https://img.shields.io/badge/Jupyter-%23F37626.svg?style=for-the-badge&logo=Jupyter&logoColor=white" /> <img alt="TensorFlow" src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white" /> <img alt="Keras" src="https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white"/>

The MNIST dataset is an acronym that stands for the Modified National Institute of Standards and Technology dataset.It is a dataset of 60,000 small square 28×28 pixel grayscale images of handwritten single digits between 0 and 9.The task is to classify a given image of a handwritten digit into one of 10 classes representing integer values from 0 to 9, inclusively. It can be simply imported from <code>Keras Datasets</code> using <code>from keras.datasets import mnist</code>

#### Explanation: How the model was trained:
The MNIST dataset comprises of a total of 60,000 28x28 images of handwrittenn single digits between 0 and 9. This 60,000 iss broken down into 48,000 and 12,000 where the former is 80% of the original training dataset and the remaining 20% of of the original training dataset using <code>from sklearn.model_selection import train_test_split</code> <code> x_train, x_val, y_train, y_val = train_test_split(
    x_train, y_train,
    test_size=0.2,       # 20% for validation
    random_state=42,     # for reproducibility
    stratify=y_train     # preserve class proportions
)</code>

#### Steps to run the code
<ul>
<li>Run the <code>Jupyter Notebook</code> named as <code>MNIST_Handwritten_DigitChecker.ipynb</code></li>
<li>The weight is saved as <code>mnist.h5</code></li>
<li>Using graphical user interface to test the model -> Run <code>gui.py</code></li>
</ul>

#### Result
<code>Test loss: 0.027963083237409597 </code> <br>
<code>Test accuracy: 0.9919999837875366</code>
