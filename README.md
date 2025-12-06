🧠 Face Recognition Attendance System – Project Description
The Face Recognition Attendance System is a Python-based desktop application designed to automate attendance marking using real-time facial recognition. Instead of manual attendance, the system identifies individuals through a live webcam feed and records their presence accurately and efficiently.
The application provides a graphical user interface (GUI) built with PyQt5, allowing users to log in, register trainees, train facial data, mark attendance, and view date-wise attendance reports. This makes the system easy to use even for non-technical users.

🔍 Face Recognition Implementation:
Face recognition is implemented using OpenCV. During the training phase, the system captures multiple face images of a trainee through the webcam. These images are converted to grayscale, cropped using Haar Cascade classifiers, and stored in a structured dataset. The collected images are then used to train an LBPH (Local Binary Patterns Histogram) face recognizer model, which is well-suited for real-time applications.
During attendance recording, the trained model compares detected faces from the live camera feed with previously trained data. If the confidence score is within the acceptable threshold, the person is recognized, and their attendance is automatically recorded in the database for the current date.

⚙️ Key Features
    •Real-time face detection and recognition using OpenCV and LBPH algorithm.
    •GUI-based trainee registration, training, attendance marking, and report viewing.
    •Automatic attendance storage with duplicate prevention for the same day.
    •SQLite database integration for secure and lightweight data storage.
    
🛠️ Technologies Used and Their Role
    •Python: Core programming language for application logic.
    •PyQt5: Used to build an interactive desktop GUI.
    •OpenCV: Handles face detection, image processing, and recognition.
    •NumPy: Used for numerical operations and image array handling.
    •SQLite: Stores attendance records in a local database.
