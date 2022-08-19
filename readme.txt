This .zip file contains all the code and data used in the project. It includes the FER 2013 dataset, completed Jupyter notebook for training, the Flask app to serve predictions, and other utility scripts. Please feel free to modify any and all aspects of the code to suit your needs.

Once you have downloaded and extracted Project.zip, make sure to install dependencies using pipenv with the provided Pipfile and execute all commands using pipenv. Also, please make sure to add the correct path to the video file in camera.py on line 11. Next, to install pipenv, the dependencies, and run the main.py file, execute the following commands from your terminal or command prompt, making sure to add the right paths where necessary:

cd \path\to\Project\

pip install pipenv

pipenv install

pipenv run python3 main.py


The hands on project on Facial Expression Recognition is divided into following tasks:

Task 1: Introduction and Overview
>Introduction to the data and and overview of the project.
>See a demo of the final product you will build by the end of this project.
>Introduction to the Rhyme interface.
>Import essential modules and helper functions from NumPy, Matplotlib, and Keras.

Task 2: Explore the Dataset
>Display some images from every expression type in the Emotion FER dataset.
>Check for class imbalance problems in the training data.

Task 3: Generate Training and Validation Batches
>Generate batches of tensor image data with real-time data augmentation.
>Specify paths to training and validation image directories and generates batches of augmented data.

Task 4: Create a Convolutional Neural Network (CNN) Model
>Design a convolutional neural network with 4 convolution layers and 2 fully connected layers to predict 7 types of facial expressions.
>Use Adam as the optimizer, categorical crossentropy as the loss function, and accuracy as the evaluation metric.

Task 5: Train and Evaluate Model
>Train the CNN by invoking the model.fit() method.
>Use ModelCheckpoint() to save the weights associated with the higher validation accuracy.
>Observe live training loss and accuracy  plots in Jupyter Notebook for Keras.

Task 6: Save and Serialize Model as JSON String
>Sometimes, you are only interested in the architecture of the model, and  you don't need to save the weight values or the optimizer.
>Use to_json(), which uses a JSON string, to store the model architecture.

Task 7: Create a Flask App to Serve Predictions
>Use open-source code from "Video Streaming with Flask Example" to create a flask app to serve the model's prediction images directly to a web interface.

Task 8: Create a Class to Output Model Predictions
>Create a FacialExpressionModel class to load the model from the JSON file, load the trained weights into the model, and predict facial expressions.

Task 9: Design an HTML Template for the Flask App
>Design a basic template in HTML to create the layout for the Flask app.

Task 10: Use Model to Recognize Facial Expressions in Videos
>Run the main.py script to create the Flask app and serve the model's predictions to a web interface.
>Apply the model to saved videos on disk.

