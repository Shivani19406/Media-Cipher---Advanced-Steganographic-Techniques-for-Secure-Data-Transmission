# 🔐 Media Cipher — Advanced Steganographic Techniques for Secure Data Transmission

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Django-4.x-green?style=for-the-badge&logo=django&logoColor=white"/>
  <img src="https://img.shields.io/badge/Steganography-LSB%20%7C%20DCT-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Security-AES%20Encryption-orange?style=for-the-badge&logo=shield&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge"/>
</p>

<p align="center">
  <b>Hide secret messages inside images, audio, and video files — invisibly and securely.</b><br/>
  A full-stack web application that combines steganography with encryption for next-level data privacy.
</p>

---

## 🌟 What is Media Cipher?

**Media Cipher** is a web-based security application that allows users to **secretly embed confidential data** (text, files) inside digital media — images, audio, and video — without any visible change to the carrier file. It leverages advanced steganographic algorithms combined with encryption to ensure **double-layer security**.

> 💡 Think of it as a digital invisible ink — your secret message is hidden in plain sight inside a photo or audio file, completely undetectable to the human eye or ear.

---

## ✨ Key Features

- 🖼️ **Image Steganography** — Hide text/data inside PNG, JPG images using LSB (Least Significant Bit) technique
- 🎵 **Audio Steganography** — Embed secret messages inside WAV/MP3 audio files
- 🎬 **Video Steganography** — Conceal data within video frames
- 🔒 **AES Encryption** — Data is encrypted before hiding, adding a second layer of protection
- 👤 **User Authentication** — Secure login/signup system with session management
- 🌐 **Django Web Interface** — Clean, responsive web UI for encode and decode operations
- 📦 **Multi-format Support** — Works across multiple media types in one platform
- 🔍 **Steganalysis Resistance** — Encoded files are visually and statistically indistinguishable from originals

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python, Django |
| Steganography | LSB Algorithm, DCT-based techniques |
| Encryption | AES (Advanced Encryption Standard) |
| Frontend | HTML5, CSS3, JavaScript |
| Database | SQLite3 |
| Image Processing | Pillow (PIL), OpenCV |
| Audio Processing | Wave, Pydub |

---

## 📂 Project Structure

```
Media-Cipher/
├── stego_app/                  # Main Django app
│   ├── views.py                # Core encode/decode logic
│   ├── models.py               # User & file models
│   ├── urls.py                 # URL routing
│   └── templates/              # HTML pages
│       ├── index.html
│       ├── encode.html
│       └── decode.html
├── Steganogrphy/               # Steganography algorithm modules
│   ├── image_stego.py          # LSB image steganography
│   ├── audio_stego.py          # Audio steganography
│   └── video_stego.py          # Video steganography
├── manage.py                   # Django project manager
├── db.sqlite3                  # SQLite database
├── requirements.txt            # Python dependencies
└── README.md
```

---

## ⚙️ How to Run Locally

### 🔧 Prerequisites
- Python 3.8+
- pip
- Virtual environment (recommended)

### 📥 Installation

```bash
# Clone the repository
git clone https://github.com/Shivani19406/Media-Cipher---Advanced-Steganographic-Techniques-for-Secure-Data-Transmission.git
cd Media-Cipher---Advanced-Steganographic-Techniques-for-Secure-Data-Transmission

# Create and activate virtual environment
python -m venv env
env\Scripts\activate        # On Windows
# source env/bin/activate   # On Mac/Linux

# Install dependencies
pip install -r requirements.txt
```

### ▶️ Run the App

```bash
python manage.py migrate
python manage.py runserver
```

Open your browser and go to: **http://127.0.0.1:8000**

---

## 🔬 How It Works

### Encoding (Hiding Data)
```
Original Media File + Secret Message
          ↓
    AES Encryption
          ↓
   LSB Steganography
          ↓
  Stego Media File (looks identical to original!)
```

### Decoding (Extracting Data)
```
Stego Media File + Password
          ↓
   LSB Extraction
          ↓
   AES Decryption
          ↓
   Original Secret Message ✅
```

---

## 🔐 Security Highlights

- **Double-layer protection**: Encryption + Steganography
- Even if the stego file is intercepted, the data remains encrypted
- LSB technique causes **less than 0.1% perceptible change** in media quality
- Password-protected encode/decode operations

---

## 🚀 Future Enhancements

- 📱 Mobile-responsive UI improvements
- ☁️ Cloud storage integration (AWS S3)
- 🧠 AI-based steganalysis detection resistance
- 🔑 RSA asymmetric key encryption support
- 📊 Stego capacity analyzer dashboard

---

## 👩‍💻 Author

**Tiragamalla Shivani**
📧 tiragamallashivani@gmail.com
🔗 [GitHub](https://github.com/Shivani19406)
🔗 [LinkedIn](https://linkedin.com/in/tiragamallashivani)

---

## 📜 License

This project is licensed under the **MIT License** — feel free to use and build on it!

---

<p align="center">
  🔐 <i>Your data, hidden in plain sight — Media Cipher keeps your secrets safe.</i>
</p>
