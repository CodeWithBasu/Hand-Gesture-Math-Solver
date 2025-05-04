# ✋📀 Hand Gesture Math Solver

An innovative **AI-powered math-solving tool** that lets you *draw equations in the air* using hand gestures — powered by **Computer Vision**, **Hand Tracking**, and **Google Gemini AI**!

---

## 🚀 Demo

> *(Add a link to a demo video or GIF here if available)*

---

## 📌 Features

* ✍️ **Draw math expressions** using your **index finger**
* 👍 **Clear canvas** using a **thumbs up gesture**
* 🖖 **Solve the expression** by showing **four fingers (excluding the pinky)**
* ✌️ **Pause or resume drawing** using **index and middle fingers together**
* 🧠 AI-generated solutions via **Google Gemini**
* 💥 Interactive UI using **Streamlit**

---

## 🛠️ Tech Stack

| Component       | Description                              |
| --------------- | ---------------------------------------- |
| `OpenCV`        | Video capture and image processing       |
| `cvzone`        | Simplified hand tracking using Mediapipe |
| `Streamlit`     | Web-based interactive interface          |
| `Google Gemini` | Math problem solver via Generative AI    |
| `PIL`           | Image conversion before sending to AI    |
| `NumPy`         | Canvas and image manipulation            |

---

## 🖼️ How It Works

1. **Hand Detection**: Detects hand landmarks using `cvzone`.
2. **Draw with Gestures**:

   * Raise **only the index finger** to draw.
   * Show **index + middle finger** to **pause/resume drawing**.
   * Show **thumbs up** to clear the canvas.
   * Show **4 fingers (excluding pinky)** to solve the equation.
3. **AI Solving**: Sends your drawn equation to **Google Gemini** for solving.
4. **Display**: The live camera feed, drawing canvas, and AI result are displayed in the **Streamlit** app.

---

## 🧑‍💻 Installation

```bash
git clone https://github.com/CodeWithBasu/Hand-Gesture-Math-Solver.git
cd hand-gesture-math-solver
pip install -r requirements.txt
```

---

## 📆 Requirements

* Python 3.7+
* Webcam
* Internet connection (for Gemini API)

**Required Python Libraries:**

```bash
opencv-python
cvzone
numpy
Pillow
streamlit
google-generativeai
```

---

## 🔐 API Key Setup

You need a [Google Generative AI API Key](https://makersuite.google.com/app).

In the script, update the line:

```python
genai.configure(api_key="YOUR_API_KEY_HERE")
```

---

## ▶️ Run the App

```bash
python -m streamlit run main.py
```

Make sure your webcam is enabled and not in use by another app.

---

## ✋ Gesture Control Guide

| Gesture                   | Action                    |
| ------------------------- | ------------------------- |
| ☝️ Index finger only      | Draw on the canvas        |
| ✌️ Index + Middle fingers | Pause/Resume drawing      |
| 👍 Thumb up               | Clear the canvas          |
| ✋ Four fingers (no pinky) | Solve using Google Gemini |

---

## 🚧 Future Ideas

* Handwriting recognition enhancement
* Multi-step math solutions
* Equation history and save options

---

## 🙌 Credits

Developed by **Basudev**
Powered by `cvzone`, `OpenCV`, `Streamlit`, and `Google Gemini API`

---

## 📄 License

This project is licensed under the **MIT License**.
