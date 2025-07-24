# Hand Gesture PPT Control

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Built With](https://img.shields.io/badge/Tech-OpenCV%20%7C%20cvzone%20%7C%20Python-blue)

Control your PowerPoint presentations **touch-free** using real-time hand gestures and a webcam. This project uses computer vision and hand tracking to let you:
- Move between slides
- Draw annotations
- Erase highlights
- All using simple finger gestures

Perfect for **teachers, presenters, or trainers** seeking a modern and contactless way to interact with slides.

---

## ✨ Features

- 👉 Navigate to **next/previous** slides using hand poses
- ✍️ **Draw** on slides using index finger
- 🧽 **Erase** annotations with a gesture
- 🔴 Display your **live webcam** in the corner of the slides
- 🖐️ All actions performed using **cvzone** hand tracking

---

## 🧠 How It Works

1. A webcam feed captures your hand in real time.
2. `cvzone.HandTrackingModule` detects finger landmarks.
3. Specific finger combinations trigger actions:

| Gesture                    | Action             |
|---------------------------|--------------------|
| 👍 Thumb Up               | Previous Slide     |
| 🤙 Pinky Up              | Next Slide         |
| ☝️ Index Finger Only      | Draw Mode          |
| ✌️ Index + Middle Fingers | Pointer Mode       |
| ✋ Three Fingers Up        | Erase Annotation   |

---

## 🛠️ Requirements

Install all dependencies with:

```bash
pip install -r requirements.txt
```

### `requirements.txt` content:

```
opencv-python
numpy
cvzone
```

---

## 📂 File Structure

```
hand-gesture-ppt-control/
├── pptControl.py                # Main application script
├── requirements.txt             # Python dependencies
├── Presentation/                # Folder with slide images (e.g., slide1.jpg, slide2.jpg)
├── docs/                        # Optional demo images/GIFs
└── README.md
```

> ✅ Ensure the `Presentation/` folder contains your presentation slides as images.  
> Accepted formats: `.jpg`, `.png`, etc.

---

## 🚀 How to Run

1. Add your slides as images inside a folder called `Presentation/`
2. Launch the script:

```bash
python pptControl.py
```

3. Position your hand in front of your webcam.
4. Use gestures to control the flow of the presentation.

---

## 📸 Demo (Optional)

> Add a screenshot or GIF of your system in action.  
> Example path: `docs/demo.gif`

---

## 📌 To-Do / Enhancements

- [ ] Add gesture for fullscreen toggle
- [ ] Voice command support
- [ ] Gesture customization menu
- [ ] Export presentation recording as video

---

## 👤 Author

**Hridey Dalal**  
📧 [hrideydalal1@gmail.com](mailto:hrideydalal1@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/hridey-/)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
