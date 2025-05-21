Facial-Recognition-System 


This project implements a face recognition system using the dlib library and pre-trained models from the face_recognition_models package. The system is capable of detecting faces in images, extracting facial landmarks, and computing facial encodings to identify or compare faces based on their similarity.

Key Features:

Face Detection:

The project supports two detection models: HOG-based detector (faster but less accurate) CNN-based detector (more accurate, especially for smaller faces, but requires GPU acceleration for optimal performance). Faces are detected and represented as bounding boxes in the image. Facial Landmark Detection:

Supports both 68-point and 5-point facial landmark predictors to capture the geometry of the face for alignment and recognition. Face Recognition:

Uses a pre-trained model to generate face encodings, which are high-dimensional feature vectors unique to each face. These encodings can be compared to calculate similarity between faces using Euclidean distance, enabling the system to identify or verify individuals. Image Handling:

Loads image files using the Pillow library and converts them into NumPy arrays for processing. Ensures that face detection bounding boxes stay within the bounds of the image. Distance Calculation:

Compares multiple face encodings to a known face encoding and returns the similarity scores, which are used to determine how closely faces match. Technologies Used:

Python: Core language for implementation. dlib: Library for face detection, shape prediction, and face encoding. Pillow (PIL): Used for loading and manipulating image files. NumPy: Handles numerical operations and array manipulation. face_recognition_models: Pre-trained models for face detection and recognition. Applications:

Identity verification for security systems. Facial recognition in photo management applications. Real-time face recognition for video surveillance. This project provides a robust, scalable solution for face recognition tasks by leveraging both classical (HOG) and deep learning (CNN) approaches, making it adaptable for different performance needs.
