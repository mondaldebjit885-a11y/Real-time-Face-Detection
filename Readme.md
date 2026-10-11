A simple and lightweight python script that detects human faces in real-time using a webcam stream or video file. The project wraps Google's **MediaPipe Face Detection** API into a Python class and includes custom drawing for face bounding boxes and FPS tracker.

---

## ✨ Features

- **Ultra-Fast Face Detection:** Uses MediaPipe's very fast face detection model.
- **Custom Bounding Boxes:** Visualizes fancy and dynamic bounding boxes around detected faces instead of regular rectangles.
- **Prediction Confidence:** Shows face detection prediction confidence percentage above detected faces.
- **FPS Counter:** Tracks and displays application performance in real-time.
- **OOP Design:** Is implemented using Object-Oriented Programming techniques (`FaceDetector` class).

---

## 🚀 Getting Started


### 1. Prerequisites
The project requires Python 3.7 or higher.



### 2. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME
cd mondaldebjit885-a11y
```


### 3. Install Required Packages
Install additional third-party libraries with `pip`:
```bash
pip install -r requirements.txt
```
*(Or `pip install opencv-python mediapipe`)*



### 4. Running the Application
By default, the script is set to capture your system's primary webcam. Just launch the script:
```bash
python face_detector.py
```
- Press **`q`** on your keyboard to close the application window.




## ⚙️ Configurations & Customizations

### Running the Detector with Pre-recorded Video
In order to switch from using the webcam to running on a pre-recorded video file, open `face_detector.py` file and go to `main()` function. Then change the following line of code:
```python
# Using the Webcam (Default)
cap = cv2.VideoCapture(0)

# Using the Local Video File (Replace with your own file path)
cap = cv2.VideoCapture("assets/sample_video.mp4")
```

### Changing Sensitivity of the Detector
You can change the detection sensitivity when creating the face detector object like below:
```python
# Only detects faces if the confidence level is 75% or more
detector = FaceDetector(minDetectionCon=0.75)
```

---

## 🛠️ Project Structure

```text
├── face_detector.py     # Application script
├── requirements.txt     # Python Dependencies for the project
└── README.md            # Documentation of the project
```

---

## 📄 LICENSE

This project is open source and available under the terms of the [MIT License](LICENSE).