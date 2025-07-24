# Hand Gesture PPT Control

This project allows users to control PowerPoint presentations using real-time hand gestures detected through a webcam. Built using OpenCV and CVZone, the system recognizes specific hand poses to navigate slides, draw on them, and erase markings without the need for a mouse or keyboard.

## Features

- Navigate to next and previous slides using hand gestures  
- Draw on the slide to highlight important content  
- Erase previous annotations with a specific gesture  
- Live video feed overlayed on the presentation window  
- Gesture detection using only a standard webcam  

## How It Works

- The webcam captures the user's hand  
- `cvzone.HandTrackingModule` detects hand landmarks  
- Finger combinations trigger specific slide control actions:
  - **Thumb up** → Previous slide  
  - **Pinky up** → Next slide  
  - **Index finger only** → Draw on slide  
  - **Index + Middle finger** → Pointer mode  
  - **Three fingers up** → Erase last annotation  

## Requirements

Install all dependencies using:

```bash
pip install -r requirements.txt
````

Dependencies:

* opencv-python
* numpy
* cvzone

## File Structure

```
hand-gesture-ppt-control/
├── pptControl.py                # Main script
├── requirements.txt             # Project dependencies
├── Presentation/                # Slide images used as presentation
├── docs/                        # (Optional) Folder for demo images or GIFs
└── README.md
```

> Note: The `Presentation/` folder must contain your presentation images (e.g., slide1.jpg, slide2.jpg...).

## How to Run

1. Place your slide images in a folder named `Presentation/`
2. Run the main script using the command below:

   ```bash
   python pptControl.py
   ```
3. Use your hand gestures in front of the webcam to control the slides.

## Demo

Add screenshots or demo GIFs in the `docs/` folder and embed them here like:

```markdown
![Demo](docs/demo.png)
```

## License

This project is licensed under the [MIT License](LICENSE).

```
