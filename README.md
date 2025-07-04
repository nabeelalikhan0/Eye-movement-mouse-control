
---

````markdown
# 👁️ Eye Blink Scroll Controller

Control your computer screen's scroll using your **eye blinks** via your webcam!

- **Left eye blink** → Scroll **down**  
- **Right eye blink** → Scroll **up**  

This project uses **OpenCV** for real-time face and eye detection and **PyAutoGUI** to simulate scrolling.

---

## 📸 Demo

https://user-images.githubusercontent.com/your-demo.gif

---

## 🧠 How It Works

- Uses Haar Cascade classifiers to detect face and eyes.
- Analyzes eye region brightness:
  - A **closed eye** appears darker than an open one.
- Scrolls up/down based on which eye is closed while the other is open.
- Has a cooldown to prevent excessive triggering.

---

## 🔧 Features

✅ Real-time eye tracking  
✅ Blink-based scrolling logic  
✅ No special hardware needed (just a webcam)  
✅ Adjustable sensitivity  
✅ Visual feedback (bounding boxes on eyes)

---

## 🚀 Getting Started

### 🔩 Dependencies

Install the required packages:

```bash
pip install opencv-python pyautogui numpy
````

### ▶️ Run the App

```bash
python eye_scroll.py
```

Press `q` to quit the window.

---

## ⚙️ Configuration

You can fine-tune the sensitivity by adjusting this parameter in the code:

```python
INTENSITY_THRESHOLD = 60  # Lower = more sensitive to blinking
```

Adjust `scroll_cooldown` (in seconds) to control how often scroll is triggered:

```python
scroll_cooldown = 1.0  # seconds between scrolls
```

---

## 🛠️ Future Improvements

* Add calibration step for more accuracy
* Use Dlib or Mediapipe for better landmark detection
* Support for left/right scrolling
* Add GUI toggle or hotkeys

---

## 🧑‍💻 Author

**Nabeel Ali Khan**
🔗 [GitHub](https://github.com/nabeel03103n)
💼 AI & ML Enthusiast | Ethical Hacker | Backend Developer

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

```
 
