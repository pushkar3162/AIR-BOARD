# AIR-BOARD
A board made to write on screen using fingers or object (pink in color) with audio commands to clear screen and (ctrl+s) to save the image



# 🖌️ Air Canvas with Voice Control & Save Functionality

A futuristic gesture-based drawing app using **Python**, **OpenCV**, and **Speech Recognition** — now enhanced to track a **pink-colored object** instead of blue. This app lets you draw on a virtual canvas using your finger or colored marker in the air, with added support for **voice commands** and **saving your artwork**.

---

## 🚀 Features

- 🎯 **Gesture-based Drawing**: Move a pink object (e.g., cap, paper, marker) in front of your webcam to draw in real time.
- 🗣️ **Voice Command Integration**: Say “clear” to instantly wipe the canvas using your microphone.
- 💾 **Save Artwork**: Press `s` to save your current canvas as a `.png` image with a timestamped filename.
- 🎨 **Multiple Drawing Colors**: Select from Blue, Green, Red, Yellow using on-screen buttons.
- ⚡ **Lag-free Performance**: Runs voice recognition in a background thread for smooth frame rate.
- 🖼️ **Real-time Mask Display**: Debug your object detection via a live HSV mask preview.

---

## 🛠️ Tech Stack

- **Python 3**
- **OpenCV** – Image capture, object detection, and drawing.
- **NumPy** – Matrix and image processing.
- **SpeechRecognition + PyAudio** – Voice command handling.
- **Threading** – Runs voice recognition asynchronously for better performance.

---

## 🧪 How It Works

1. **Object Detection**: Uses hardcoded HSV values to detect a pink-colored object.
2. **Tracking & Drawing**: Tracks the object's position and draws lines as it moves.
3. **Control Buttons**: Clickable zones at the top allow color switching and canvas clearing.
4. **Voice Listener**: Continuously listens for the word “clear” and resets the canvas.
5. **Save Art**: Simply press `s` and the canvas is saved with a unique filename.

---

## 🖥️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/air-canvas-voice
cd air-canvas-voice
pip install opencv-python numpy SpeechRecognition pyttsx3 pyaudio
python board.py


