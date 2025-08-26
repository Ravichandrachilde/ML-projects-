#### Handwritten Digit Classification using MLP (Scikit-learn)



This project demonstrates how to build and train a Multi-Layer Perceptron (MLP) neural network model using Scikit-learn on the classic Handwritten Digits dataset.

The goal is to recognize handwritten digits (0–9) based on pixel intensity features of small 8x8 grayscale images.



##### 🚀 Project Overview



Dataset: Handwritten Digits dataset from sklearn.datasets.



Model: Multi-Layer Perceptron (MLPClassifier).



###### Libraries Used:



scikit-learn (for ML models and metrics)



matplotlib (for data visualization)



numpy (for numerical operations)



###### The project covers:



Loading and exploring the digits dataset.



Visualizing digits using Matplotlib.



Flattening 8x8 images into 64-feature vectors.



Splitting data into training (1000 samples) and testing (remaining samples).



Training an MLP model using Stochastic Gradient Descent (SGD).



Evaluating performance using accuracy score.



###### 📂 Dataset Details



Samples: 1797 handwritten digit images.



Image size: 8×8 pixels (64 features per image).



Classes: 10 (digits 0–9).



Example visualization:



plot\_multi(0)   # Displays a batch of 16 digits



###### ⚙️ Model Architecture



Input layer: 64 nodes (flattened 8x8 image).



Hidden layers: One hidden layer with 15 neurons.



Activation function: Logistic (sigmoid).



Optimizer: Stochastic Gradient Descent (SGD).



Learning rate: 0.1.



Regularization (alpha): 1e-4.



###### 📊 Training Results



Training stops when loss no longer improves.



Loss curve visualization:



fig, axes = plt.subplots(1, 1)

axes.plot(mlp.loss\_curve\_, 'o-')

axes.set\_xlabel("Number of Iterations")

axes.set\_ylabel("Loss")

plt.show()



✅ Model Evaluation



Test Accuracy: ~91.4%



from sklearn.metrics import accuracy\_score

accuracy\_score(y\_test, predictions)   # Output: 0.9146





The model generalizes well and achieves human-level performance on the downscaled dataset.



###### 📦 Installation \& Usage



Clone the repository and install the required libraries:



git clone https://github.com/your-username/digit-mlp-classifier.git

cd digit-mlp-classifier



\# install dependencies

pip install -r requirements.txt





Run the Jupyter notebook or Python script:



jupyter notebook digit\_mlp\_classifier.ipynb



###### 📚 Dependencies



Python 3.x



scikit-learn



matplotlib



numpy



###### Install them using:



pip install scikit-learn matplotlib numpy

