# Steganography-Tool

This is a Flask-based steganography tool that allows users to hide and extract secret messages within images (PNG, JPG, JPEG), audio (WAV), and video (MP4) files. It also includes encryption and decryption using a password for added security.

##  Features

- **Image Steganography** – Hide messages inside image files using LSB (Least Significant Bit) encoding.
- **Audio Steganography** – Encode messages into audio files without affecting sound quality.
- **Video Steganography** – Store secret messages within video frames.
- **Encryption & Decryption** – Uses SHA-256 hashing and XOR encryption for secure message storage.
- **User-Friendly Web Interface** – Upload files and retrieve hidden messages easily.

##  Technologies Used

- **Flask** – Web framework for building the application.
- **PIL (Pillow)** – For image processing.
- **OpenCV** – Handling video frames for steganography.
- **Wave Module** – Processing audio files.
- **Hashlib** – Secure message encryption.

##  How to Use This Steganography Tool

###  1. Installation & Setup

####  Clone the Repository:
```bash
git clone https://github.com/yourusername/steganography-tool.git
cd steganography-tool
```

#### ~ Install Dependencies:
```bash
pip install -r requirements.txt
```

#### ~ Run the Flask App:
```bash
python app.py
```
The application will start at **http://127.0.0.1:5000/**.

---

###  2. Encoding a Message (Hiding Data)

1. Open the web interface by visiting **http://127.0.0.1:5000/**.
2. Click on **"Encode"** and upload an **image (PNG, JPG, JPEG), audio (WAV), or video (MP4)** file.
3. Enter your **secret message** and set a **password** for encryption.
4. Click **"Encode"** and download the modified file.

---

###  3. Decoding a Message (Extracting Data)

1. Go to **http://127.0.0.1:5000/decode**.
2. Upload the **modified file** that contains the hidden message.
3. Enter the **correct password** used during encoding.
4. Click **"Decode"** to retrieve the secret message.

---

###  4. Notes & Tips

 Use **lossless formats** like PNG (images) and WAV (audio) for best results.
 The message size **should not exceed the file’s capacity**.
 If decoding fails, ensure you are using the **correct password**.

🔗 **Ready to Try?** Clone the repo & start hiding messages today! 🚀
