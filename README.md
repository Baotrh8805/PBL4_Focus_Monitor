# 📊 AI-Powered Attendance & Focus Monitoring System

This is a Python project using **Computer Vision and AI** to:
- Automatically take student attendance using facial recognition
- Monitor student focus during class sessions
- Store history, statistics, and generate reports

---

## 🚀 Main Features

- 📷 Real-time facial recognition via camera
- 👥 Student management (add / edit / delete)
- 📝 Create class sessions, automatic attendance, and focus scoring
- 📚 Session history tracking
- 📊 Focus level statistics
- 🧠 Student behavior analysis (AI)

---

## 🛠 Technologies Used

- Python 3.11
- OpenCV
- CustomTkinter / Tkinter
- MySQL
- YOLO (face detection)
- Face Recognition (embedding)
- NumPy, Pillow

---

## 📁 Project Structure

```
PBL4_Focus_Monitor/
    │──code/
        │── app_main.py
        │── ai_summarizer.py
        │── behavior_analyzer.py
        │── focus_manager.py
        │── recognition_engine.py
        │── login.py
        │── hash_password.py
        │── email_service.py
        │── home.py
        │── camera.py
        │── hocsinh.py
        │── lichsu.py
        │── chitiet.py
        │── thongke.py
        │── database.py
        │── data_loader.py
        │── faces_db.npz
        │── faces_db_images/
        │── image/
        │── student_avatars/
        │── remember.txt
    │── data.yaml
    │── README.md
    │── .gitignore
    │── requirements.txt
    │── venv/ (auto-generated)
    │── weights/
        │──best.pt
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone repository
```bash
git clone https://github.com/Baotrh8805/PBL4_Focus_Monitor.git
cd PBL4_Focus_Monitor
```

### 2️⃣ Install Python
- Install Python 3.11 (recommended for this project)

### 3️⃣ Run the following commands
```bash
py -3.11 -m venv venv
venv\Scripts\activate     # On Windows
# or
source venv/bin/activate  # On macOS/Linux

pip install -r requirements.txt                         
python -m pip install --upgrade pip
```

### 4️⃣ Configure the following files:

**In `email_service.py`:**
```python
EMAIL = "your_email@gmail.com"
APP_PASSWORD = "your_app_password"
```

**In `ai_summarizer.py`:**
```python
GEMINI_API_KEY = "your_gemini_api_key"
```

**In `database.py`:**
```python
DB_CONFIG = {
    'host': 'localhost',          # Or MySQL server IP
    'user': 'root',               # Your MySQL username
    'password': 'your_password',  # Your MySQL password  
    'database': 'giamsatatt'      # Database name
}
```

### 5️⃣ Run the application
```bash
python code/app_main.py
```

---

## ⚠️ Important Notes

1. The `venv/` folder is not pushed to GitHub
2. 📦 Model Files
    - YOLO model files (`best.pt`, `last.pt`, `yolov8n-face-lindevs.pt`, `yolov8s-face-lindevs.pt`) are not pushed to GitHub
    - Please train or download the model and place it in the `weights/` folder
3. Files `faces_db.npz` and face images are for local use only
4. MySQL database configuration is required before running the application

