# Hand-Written-Digit-Recognition-in-python-Django

This repository contains a Django web application for recognizing handwritten digits using a Convolutional Neural Network (CNN) model. The model is trained on the MNIST dataset and saved in an .h5 file format. The application allows users to upload an image of a handwritten digit, converts the image into an Excel format, and passes it to the trained model to predict the digit.

Features
Image Upload: Users can upload an image of a handwritten digit.
Image Processing: The uploaded image is processed and converted into an Excel format suitable for model input.
Digit Prediction: The processed image data is passed to the trained CNN model to predict the digit.
Model: The CNN model is trained on the MNIST dataset and stored as an .h5 file.
Requirements
Python 3.x
Django 3.x
TensorFlow 2.x
NumPy
OpenCV
Pandas
Installation
Clone the repository:

git clone https://github.com/soursecodee000/Hand-Written-Digit-Recognition-in-python-Django.git
cd Hand-Written-Digit-Recognition-in-python-Django

Create and activate a virtual environment

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

Install the required packages
pip install -r requirements.txt

Apply the Django migrations:
python manage.py migrate

Start the Django development server:
python manage.py runserver

Usage
Open your web browser and go to http://127.0.0.1:8000/.
Upload an image of a handwritten digit.
The app will process the image, convert it to an Excel format, and predict the digit using the trained CNN model.
Project Structure
digit_recognition/ - Django project directory.
recognition/ - Django app for digit recognition.
models.py - Contains the definition of the CNN model.
views.py - Handles the image upload and processing.
urls.py - URL routing for the app.
templates/ - HTML templates for the app.
static/ - Static files (CSS, JavaScript, images).
media/ - Uploaded images.
trained_model/ - Directory containing the trained .h5 model file.
requirements.txt - List of Python packages required for the project.
Model Training
The model is a Convolutional Neural Network trained on the MNIST dataset. The training script (not included in this repository) converts the MNIST dataset to an Excel format before training. The trained model is saved as model.h5 and used for prediction in the Django app.

Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

