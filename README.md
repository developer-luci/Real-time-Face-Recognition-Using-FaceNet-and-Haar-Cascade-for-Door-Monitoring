Real-time Face Recognition Using FaceNet and Haar Cascade for Door Monitoring
This project implements real-time face recognition using the FaceNet model and Haar Cascade for door monitoring. The system detects and recognizes faces using a webcam or video feed, comparing detected faces against a database of known faces to grant or deny access.

Overview
The project consists of several components:

Training.ipynb: Jupyter Notebook used to train the FaceNet model and create a face database using known face images.
Monitoring.ipynb: Jupyter Notebook for real-time face recognition using the trained FaceNet model and Haar Cascade face detection.
index.php: PHP script for handling user registration and login functionalities.
db.php: PHP script for database connection and user authentication.
main.php: PHP script to display a gallery of detected unknown faces.
script.js: JavaScript file to handle form slide animations in the login/signup page.
style.css: CSS stylesheet for styling the login/signup page.
Components
Training (Training.ipynb)
Trains the FaceNet model using images of known individuals.
Generates face embeddings for known faces.
Creates a database (data.pkl) of known face embeddings.
Monitoring (Monitoring.ipynb)
Implements real-time face recognition using a webcam or video feed.
Detects faces using Haar Cascade and extracts face embeddings using the FaceNet model.
Compares face embeddings against the known face database to recognize individuals.
Captures and saves images of unknown faces detected during monitoring.
Sends email notifications with images of unknown faces to the system owner.
User Authentication (index.php, db.php)
index.php: Implements a login/signup form for user authentication.
Users can register by providing an email, mobile number, and password.
Registered users can log in using their email and password.
db.php: Handles database connection and user authentication logic.
Frontend (main.php, script.js, style.css)
main.php: Displays a gallery of detected unknown faces.
script.js: Handles form slide animations for login/signup interaction.
style.css: Stylesheet for the login/signup form and gallery display.
Usage
Training: Use Training.ipynb to train the FaceNet model and create a database of known face embeddings.
Monitoring: Run Monitoring.ipynb for real-time face recognition and monitoring using a webcam or video feed.
User Authentication: Use index.php and db.php for user registration and login functionalities.
Frontend: Modify main.php, script.js, and style.css for customizing the login/signup form and gallery display.
Requirements
Python 3.x
Jupyter Notebook
OpenCV
Keras
PHP
MySQL or MariaDB
Web server (e.g., Apache)
Setup
Install the required Python libraries (opencv-python, keras, numpy, PIL, numpy, matplotlib, keras-facenet).
Set up a web server with PHP and MySQL/MariaDB support.
Create a database and configure the database connection in db.php.
Customize the frontend (main.php, script.js, style.css) according to your design preferences.
Run Training.ipynb to train the FaceNet model and create the face database.
Run Monitoring.ipynb for real-time face recognition and monitoring.
Credits
FaceNet model implementation: keras-facenet
Face detection: OpenCV Haar Cascade
License
This project is licensed under the MIT License.
