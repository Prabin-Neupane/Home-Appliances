# 🤖 Gesture-Controlled Device Switching with Arduino and OpenCV

This project uses **hand gesture recognition** via webcam and **Arduino with relays** to control external devices. By counting the number of fingers shown to the camera, you can turn ON/OFF up to 5 devices connected via relays. It's a simple and interactive way to control your home or IoT devices without physical contact.

---

## ✨ Features

- Real-time hand tracking using webcam.
- Recognizes the number of fingers (0 to 5).
- Controls 5 digital output pins on Arduino.
- Works with external devices through relays (e.g., bulbs, fans, etc.).

---

## 🛠️ Requirements

### 🧰 Hardware:
- Arduino board (e.g., Uno, Nano)
- Relay module (up to 5 channels)
- External devices (bulb, fan, etc.)
- Jumper wires
- USB cable for Arduino

### 💻 Software:
- Python 3.8.10
- [cvzone](https://github.com/cvzone/cvzone) (uses OpenCV under the hood)
- OpenCV (`cv2`)
- pyfirmata (for Arduino communication)

---

## 📦 Installation & Setup

### 1. 🔌 Arduino Setup
- Connect the Arduino to your PC via USB.
- Note the COM port (e.g., `COM4`) — update this in `controller.py`.

### 2. ⚡ Relay Wiring
- Connect relay IN1–IN5 to Arduino pins: 12, 10, 8, 6, and 4.
- Connect your external devices to relays.

### 3. 🐍 Python Environment Setup

```bash
# Install required packages
pip install opencv-python cvzone pyfirmata

