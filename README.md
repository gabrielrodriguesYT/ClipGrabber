# 🎬 ClipGrabber (Frontend)

ClipGrabber is a **web-based frontend** designed to work together with **ClipGrabber-API**, allowing users to download YouTube videos through a simple and user-friendly interface.

⚠️ **Important**: This frontend depends on the backend running **locally**. If the backend is hosted online, YouTube may block downloads.

---

## 📌 Features

* Clean and simple web interface
* Connects to a local Python backend (ClipGrabber-API)
* Supports YouTube video downloads
* Works on modern browsers

---

## 🧠 How it works

1. The user pastes a YouTube video URL
2. The frontend sends a request to the local backend API
3. The backend processes the download using `yt-dlp`
4. The video is returned/downloaded to the user

---

## 📂 Project structure

```
ClipGrabber/
├── index.html
└── README.md
```

---

## 🛠️ Requirements

* A modern web browser (Chrome, Firefox, Edge)
* **ClipGrabber-API running locally**

---

## 🔽 Clone the repository

```bash
git clone https://github.com/gabrielrodriguesYT/ClipGrabber.git
cd ClipGrabber
```

---

## 🔗 Backend configuration (VERY IMPORTANT)

The frontend must point to the **local backend URL**.

### 1️⃣ Open the JavaScript configuration file

Example:

```js
  fetch("https://back_end/download", { //replace with back end url
```

### 2️⃣ Change it if necessary

Make sure the URL and port match the backend configuration in `ClipGrabber-API`.

---

## ▶️ Running the frontend

You can run the frontend in two ways:

### Option 1 — Open directly in the browser

Simply open:

```
index.html
```

in your browser.

---

### Option 2 — Local HTTP server (recommended)

#### Using Python

```bash
python -m http.server 8080
```

Then open:

```
http://localhost:8080
```

---

## 🔄 Running with the backend

1. Start the backend:

```bash
cd ClipGrabber-API
source venv/bin/activate  # Linux/macOS
python main.py
```

2. Start the frontend
3. Paste a YouTube URL
4. Download the video

Complete tutorial:https://github.com/gabrielrodriguesYT/ClipGrabber-API/

---

## ⚠️ Known limitations

* ❌ Does not work without the backend
* ❌ Does not work if the backend is hosted online
* ❌ YouTube may block cloud IPs
* ✅ Fully functional on localhost

---

## 🔒 Security notes

* Never expose the backend API publicly
* Always use localhost
* Do not hardcode secrets

---

## 📄 License

This project is provided for **educational purposes only**.

---

## 👤 Author

**Gabriel Rodrigues**
GitHub: [https://github.com/gabrielrodriguesYT](https://github.com/gabrielrodriguesYT)

---

⭐ If you like this project, consider giving it a star on GitHub!
