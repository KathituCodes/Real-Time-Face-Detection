# 🎯 Real-Time Face Detection with Streamlit & OpenCV

This project is a real-time face detection web application built using **OpenCV**, **Streamlit**, and the **Viola-Jones (Haar Cascade)** algorithm.

## 📸 Live Demo

Run the app locally by executing:

```bash
streamlit run app.py
```

---

## 📂 Project Structure

```
├── app.py                   # Main Streamlit app with enhanced features
├── facial_recognition.py    # Original baseline face detection app
├── haarcascade_frontalface_default.xml  # Pre-trained Haar Cascade model
```

---

## 🧠 How It Works

The system uses OpenCV’s Haar cascade classifier to detect human faces in real-time through a webcam. It then overlays rectangles around detected faces on the video stream.

---

## 🚀 Features

### ✅ Baseline Version (`facial_recognition.py`)

* Real-time webcam face detection
* Uses OpenCV’s built-in Haar Cascade classifier
* Fixed parameters: `scaleFactor=1.3`, `minNeighbors=5`
* Static green rectangle as overlay
* Stop detection only by pressing Streamlit “Stop” button

---

### 🌟 Enhanced Version (`facial.recog2.py`)

**Major Improvements:**

1. **🖍️ Customizable Detection Settings:**

   * Dynamic sliders to control:

     * `scaleFactor`: controls image size reduction between scans
     * `minNeighbors`: controls how many neighbors are needed to retain a detection
   * Offers greater flexibility and performance tuning.

2. **🎨 Custom Rectangle Colors:**

   * Integrated a color picker to allow users to choose the color of the face detection rectangle overlay in real time.

3. **⚡ Streamlined UX:**

   * Clearly labeled buttons and titles.
   * Clean and responsive UI using `st.empty()` for continuous image rendering.
   * Improved color conversion logic for accurate color rendering from HEX to BGR.

---

## 🔧 Requirements

Install dependencies with:

```bash
pip install opencv-python streamlit
```

---

## 📥 How to Run

1. Clone the repository:

```bash
git clone https://github.com/yourusername/facial-recognition-app.git
cd facial-recognition-app
```

2. Run the Streamlit app:

```bash
streamlit run app.py
```

---

## 📌 Notes

* Make sure your webcam is accessible and not being used by other applications.
* `haarcascade_frontalface_default.xml` is loaded directly from OpenCV’s built-in data, but you can replace it with your own trained model if needed.

---



