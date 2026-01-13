# Face-Detection-Recognition-

# Face Recognition System using OpenCV & KNN

This project implements a real-time face recognition system inside a Jupyter Notebook. It captures face images from a webcam, trains a K-Nearest Neighbors (KNN) classifier, and performs live face recognition and image-based recognition.

---

## How to Use

### Step 1 — Run All Cells in Order
Open the notebook and execute each cell sequentially from top to bottom.

---

### Step 2 — Capture Face Images
When prompted:

Enter Name: your_name

The system will automatically capture up to 50 face images using your webcam.

Press ESC to stop capturing early.

---

### Step 3 — Model Training
The notebook automatically trains the KNN model using the captured face images.

If successful, you will see:

Model trained on X samples.

---

### Step 4 — Real-Time Face Recognition
The webcam window opens and starts recognizing faces in real time.

Press ESC to close the window.

---

### Step 5 — Recognize Faces from Image
When prompted:

Enter image path: path_to_image.jpg

The system detects faces in the image and displays the recognized names.

---

## How It Works

- Face detection uses Haar Cascade Classifier
- Faces are converted to grayscale, resized to 100×100, and flattened
- A KNN classifier is created using:
  
  model = KNeighborsClassifier(n_neighbors=3)

- The model is trained using:
  
  model.fit(X, y)

- Predictions are performed using:
  
  model.predict(face)

---

## Notes

- Capture more images for better accuracy
- Ensure proper lighting for improved recognition
- Designed for educational and learning purposes

---

