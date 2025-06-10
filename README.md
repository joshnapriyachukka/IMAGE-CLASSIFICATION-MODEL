# IMAGE-CLASSIFICATION-MODEL

COMPANY: CODTECH IT SOLUTIONS

NAME: CHUKKA JOSHNA PRIYA

INTERN ID: CT04DN841

DOMAIN: MACHINE LEARNING

DURATION: 4 WEEKS

MENTOR: NEELA SANTOSH

##

As part of my internship at CodTech IT Solutions in the Machine Learning domain, I developed an image classification system using a Convolutional Neural Network (CNN) trained on the CIFAR-10 dataset. The objective was to design a simple desktop-based application that allows users to select any image and get a prediction of the object category it belongs to, using a trained deep learning model.

The application was developed using Python, integrating libraries such as TensorFlow and Keras for building and training the CNN, Pillow for image handling, NumPy for array operations, and Tkinter for GUI development.

1. Dataset and Model Training
The CIFAR-10 dataset, which consists of 60,000 color images (32x32 pixels) across 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck), was used for training the model. The dataset was automatically downloaded using tensorflow.keras.datasets.cifar10.

After loading the dataset, the images were normalized (scaled between 0 and 1) to improve training performance. The CNN model was built with three convolutional layers, each followed by max-pooling, and ending with two dense layers including the final classification layer with a softmax activation function to output probability scores for 10 categories.

The model was compiled with the Adam optimizer and sparse categorical crossentropy loss function. It was trained for 10 epochs with a 10% validation split. After training, the model was evaluated on the test dataset to measure its accuracy and saved as cnn_model.h5 for future predictions.

2. Prediction Functionality
The application includes a prediction function that takes an image file path as input. It resizes the image to 32x32 pixels, normalizes the pixel values, reshapes it to match the input format of the CNN, and then uses the trained model to predict the class. The predicted label is matched with a predefined list of class names and returned as output.

3. GUI Interface with Tkinter
The project includes a simple graphical user interface using Tkinter:

A "Select Image" button allows the user to browse and choose any image file from their system.

Once an image is selected, it is resized and displayed in the interface.

The prediction result is shown just below the image with a label such as "Prediction: Dog" or "Prediction: Airplane".

If the trained model does not exist, it is automatically trained the first time the app is run.

This GUI made it possible to turn a complex deep learning model into a beginner-friendly tool for demonstrating how image classification works in real time.

##

#OUTPUT

![Image](https://github.com/user-attachments/assets/d3da8c98-d15b-4ef6-bf7d-63f643d85045)
![Image](https://github.com/user-attachments/assets/d4d090e8-c4d4-4ab6-b862-22cfadaf806a)
