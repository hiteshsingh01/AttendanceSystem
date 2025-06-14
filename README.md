# 🎯 Face Recognition Attendance System

This project is a real-time face recognition attendance system built using **OpenCV** and **DeepFace**. It detects faces via webcam, matches them with a pre-stored image dataset, and marks attendance in a CSV file. Unknown faces are saved separately for review.

---

## 📦 Features

- 👤 Real-time face recognition using DeepFace  
- 🧠 Uses `VGG-Face` model and OpenCV’s Haar cascades  
- ✅ Automatically marks attendance in a CSV file  
- 🕵️‍♂️ Saves unknown faces separately  
- 🔒 Prevents multiple face entries simultaneously  

---

## 🧰 Tech Stack

- Python 3.x  
- OpenCV (`cv2`)  
- DeepFace  
- Pandas  
- Haar Cascade (for fast initial face detection)  

---

## 📁 Folder Structure

```

├── images/              # Folder containing known face images (students)
├── unknown\_faces/       # Folder where unknown faces will be stored
├── attendance.csv       # Output attendance file
├── main.py              # Main Python script (your code)

````

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/hiteshsingh01/FaceAttendanceSystem.git
cd FaceAttendanceSystem
````

### 2. Install Dependencies

```bash
pip install opencv-python deepface pandas
```

### 3. Setup Known Faces

* Add images of known individuals (students) in the `images/` folder.
* File name (without extension) will be treated as the student’s name.
  *(Example: `john.png` → **john**)*

### 4. Run the Application

```bash
python main.py
```

* Press `q` to quit the webcam.
* Attendance gets recorded in `attendance.csv`.
* Unknown faces are saved in the `unknown_faces/` folder.

---

## 📌 Notes

* Ensure only **one face** appears at a time on the webcam.
* All data is stored locally — no cloud or server needed.
* Works best in good lighting conditions.

---

## 📷 Sample Output

```csv
Student Name,Time,Date,Program
john,10:45:12,2025-06-14,The Creator
unknown_1,10:47:33,2025-06-14,Unknown Entry
```

---

## 🙌 Credits

* Face Recognition: [DeepFace](https://github.com/serengil/deepface)
* Face Detection: OpenCV Haar Cascades

---

## 📜 License

This project is open-source and free to use for educational or personal purposes.

