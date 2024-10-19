Hand and Face Detection App
This project is a real-time hand and face detection application using MediaPipe, OpenCV, and Streamlit. The app captures video from a webcam, detects hands and faces in real-time, and provides voice announcements of the detected objects using gTTS. Additionally, you can upload images for hand and face detection, which the app processes and displays with annotations.

Features
Real-time detection of faces and hands using a webcam feed.
Voice announcements of the number of faces and hands detected using Google Text-to-Speech (gTTS).
Image upload support for hand and face detection in uploaded images.
Bounding boxes drawn around detected faces and hands.
Uses MediaPipe for hand detection and OpenCV’s Haar cascades for face detection.
Technologies Used
Python
OpenCV for computer vision and image processing.
MediaPipe for hand detection.
gTTS (Google Text-to-Speech) for text-to-speech voice announcements.
Streamlit for web-based GUI.
Pillow for image processing.
Pyngrok to expose Streamlit app using secure tunnels for web access.
Installation
To run this project locally, follow the steps below:

Clone the repository:

bash
Copy code
git clone https://github.com/your-username/face-detection-app.git
cd face-detection-app
Install required libraries:

Run the following command to install all dependencies:

bash
Copy code
pip install -r requirements.txt
Alternatively, install individual packages:

bash
Copy code
pip install opencv-python mediapipe gtts streamlit pyngrok Pillow
Run the Streamlit app:

bash
Copy code
streamlit run app.py
Expose the app via ngrok (Optional):

If you want to expose your local app to the internet, use Pyngrok:

bash
Copy code
!ngrok authtoken your-ngrok-token
!ngrok http 8501
How to Use
Image Upload: You can upload an image to detect hands and faces. The app will process the image, display the result with bounding boxes, and announce the count of detected hands and faces.

Real-Time Detection: The app streams real-time video, detects hands and faces in the video, and provides voice announcements when the number of detected faces or hands changes.

Voice Announcements: The app announces changes in the number of detected objects (faces and hands) using gTTS. If you enable this option, the app will speak out loud the detected counts.

Project Structure
app.py: The main script that handles the hand and face detection, image upload, and real-time video capture.
requirements.txt: The list of required libraries.
FaceDetection01.ipynb: Jupyter notebook with code for initial development and testing.
README.md: Project documentation (this file).
Future Enhancements
Custom voice options: Allow users to customize the voice for announcements.
Mobile support: Optimize for mobile devices and add functionality for detecting faces and hands from mobile cameras.
Detection improvement: Add support for more complex gestures and facial landmarks.
License
This project is licensed under the MIT License - see the LICENSE file for details.
