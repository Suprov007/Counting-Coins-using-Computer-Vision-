# Counting Coins Using Computer Vision with Flask

A Python project that uses **OpenCV** and **cvzone** to detect coins from a webcam, calculate their total value, and display the result on a **Flask web interface**.

---

## 🔹 Features

- Detect coins using a webcam.
- Identify coin values based on size and color.
- Send the calculated total to a Flask backend.
- View the latest coin sum on a web page.
- Easy to extend for different coin types or currencies.

---

## 🛠️ Technologies Used

- Python 3.x
- OpenCV
- cvzone
- Flask
- Flask-SocketIO (optional for real-time updates)
- Flask-Sock
- NumPy
- Requests

---

## 📂 File Structure

```
├── app.py                 # Flask backend
├── coin_detector.py       # Computer vision script for detecting coins
├── templates/
│   ├── index.html         # Home page
│   └── coinCount.html     # Displays the latest coin sum
├── requirements.txt       # Python dependencies
└── README.md
```

---

## ⚙️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/YourUsername/Counting-Coins-using-Computer-Vision.git
cd Counting-Coins-using-Computer-Vision
```

2. **Create a virtual environment**
```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

---

## 🚀 Running the Project

1. **Start the Flask backend**
```bash
python app.py
```
- This starts the server at `http://127.0.0.1:5000`.

2. **Start the Computer Vision script**
```bash
python coin_detector.py
```
- Opens your webcam, detects coins, and sends the total coin value to the Flask server.

3. **Open your browser**
- Home page: [http://127.0.0.1:5000/](http://127.0.0.1:5000/)
- Coin count page: [http://127.0.0.1:5000/coinCount](http://127.0.0.1:5000/coinCount)

> ⚠️ Make sure the Flask server is running **before** starting the CV script.

---

## 📦 requirements.txt

```
flask
flask-socketio
flask-sock
opencv-python
cvzone
numpy
requests
```
(Optional for debugging or plotting: `matplotlib`, `jupyter`)

---

## 🖼️ Screenshots

*(You can add images of the webcam detection and web interface here.)*

---

## ⚡ Notes

- The coin count updates in the session; you need to refresh `/coinCount` to see the latest value.  
- You can extend this project to support **live updates** using Socket.IO for real-time display.

---

## 🔗 Author

**YourWasik** – [GitHub](https://github.com/Suprov007)

