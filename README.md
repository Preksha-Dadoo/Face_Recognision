# Face Detection Using OpenCV

This project demonstrates a simple **real-time face detection** system using OpenCV and Haar Cascade classifiers. It captures video from your webcam and detects faces in live video frames, highlighting them with green rectangles.

---

## Requirements

- Python 3.6 or above
- OpenCV (`cv2`)

Install OpenCV if you don't have it yet:

```bash
pip install opencv-python
```

---

## How It Works

- The Haar Cascade classifier detects faces in grayscale images.
- The webcam feed is continuously read frame-by-frame.
- Detected faces are highlighted with green rectangles.
- Press **'a'** key to exit the program.

---

## Project Structure

- **haarcascade_frontalface_default.xml**: Pre-trained model for face detection.
- **face_detection.py**: Main Python script (your code).

---

## How To Run

1. Make sure your webcam is working.
2. Ensure you have the Haar Cascade file at the correct path (you can also use the default one from OpenCV's installed directory).
3. Run the script:

```bash
python face_detection.py
```

4. A window will open showing live video with detected faces outlined in green rectangles.
5. Press **'a'** to close the window.

---

## Notes

- If you get errors related to the XML file path, you can replace it with:

```python
cv2.data.haarcascades + 'haarcascade_frontalface_default.xml'
```

Example:

```python
face_cap = cv2.CascadeClassifier(cv2.data.haarcascades + 'haarcascade_frontalface_default.xml')
```

- Make sure lighting conditions are good for better face detection.
- You can adjust `scaleFactor` and `minNeighbors` for better accuracy if needed.

---

## License

This project is for educational purposes.
