# 📌 Face Recognition Attendance System 🎯

## 🚀 Overview
This project is a **Face Recognition-based Attendance System** built using Python, OpenCV, and the `face_recognition` library.  
It captures real-time video, detects faces, recognizes known individuals, and automatically marks attendance in a CSV file with timestamps.

---

## 🧠 Features

- 🎥 Real-time face detection using webcam  
- 🧑‍💻 Face recognition using pre-trained images  
- 📝 Automatic attendance marking in CSV  
- ⏱️ Date & time logging  
- 📂 Daily attendance file generation  
- ⚡ Fast and efficient using optimized face encodings  

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Libraries:**  
  - OpenCV (`cv2`)  
  - face_recognition  
  - NumPy  
  - CSV  
  - datetime  

---

## 🧩 System Workflow

```
Webcam → Capture Frame → Detect Face → Encode Face
       → Compare with Known Faces → Identify Person
       → Mark Attendance → Save in CSV File
```

---

## 📂 Project Structure

```
Face-Recognition-Attendance/
│── images/
│   ├── ravi.jpg
│   ├── ashutosh.jpg
│
│── main.py
│── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Install Dependencies

```bash
pip install opencv-python face_recognition numpy
```

---

### 2️⃣ Add Known Faces

- Place images inside the project folder
- Update file paths in code:
```python
face_recognition.load_image_file("path_to_image")
```

---

### 3️⃣ Run the Project

```bash
python main.py
```

---

## 📊 Output

- A CSV file will be created with current date:
```
YYYY-MM-DD.csv
```

- Example:
```
ravi, 10-32-15
ashutosh, 10-35-20
```

---

## ⚠️ Issues in Current Code (Important Fixes)

- ❌ File path uses single `\` → should use raw string:
```python
r"C:\MY PICTURES\image.jpg"
```

- ❌ Same image used for both persons  
- ❌ `if name is students:` → should be:
```python
if name in students:
```

- ❌ `now` is not updated inside loop → move inside loop:
```python
now = datetime.now()
```

---

## 🚧 Future Improvements

- Face mask detection  
- GUI (Tkinter / Streamlit)  
- Database integration (MySQL/Firebase)  
- Mobile app integration  
- Cloud-based attendance system  

---

## 📧 Contact

**Ravi Kumar**  
(Add your GitHub / LinkedIn here)

---

## ⭐ Acknowledgements

- face_recognition library  
- OpenCV community  
