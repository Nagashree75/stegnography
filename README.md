# stegnography
Steganography project in C for hiding and extracting secret messages in images.

# 🔐 Steganography Project (C Language)

## 📌 Overview
This project implements **Steganography**, a technique used to hide secret data inside another file (like an image) without visibly changing it.

The main goal is to securely embed and extract hidden messages using simple algorithms in **C programming**.

---

## 🚀 Features
- Hide secret text inside an image file
- Extract hidden text from the encoded image
- Works with BMP image format
- Simple and efficient implementation
- Command-line based execution

---

## 🛠️ Technologies Used
- C Programming
- File Handling
- Bit Manipulation
- Standard Libraries (`stdio.h`, `stdlib.h`, etc.)

---

## 📂 Project Structure

---

## ⚙️ How It Works
### Encoding:
1. Take a cover image (BMP format)
2. Read the secret message
3. Modify the least significant bits (LSB) of image pixels
4. Save the encoded image

### Decoding:
1. Read the encoded image
2. Extract bits from pixel data
3. Reconstruct the hidden message

---

## 🧑‍💻 How to Run

### 🔹 Compile
```bash
gcc encode.c -o encode
gcc decode.c -o decode

./encode input.bmp secret.txt output.bmp

./decode output.bmp extracted.txt
