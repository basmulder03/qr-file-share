# QR File Share 📱

A simple, client-side web application that allows you to share files instantly using QR codes. Upload a file, generate a QR code, and download it on any other device!

## 🌟 Features

- **File Upload**: Drag & drop or click to upload any file
- **QR Code Generation**: Instantly generates a QR code for your file
- **File Compression**: Automatically compresses files larger than 100KB using gzip compression
- **Base64 Encoding**: Files are encoded in base64 and embedded in the URL
- **URL Shortening**: Automatically shortens long URLs using TinyURL API when needed
- **Cross-Device Sharing**: Scan the QR code or share the link to download on another device
- **No Server Required**: Everything runs in the browser - your files never leave your device
- **Responsive Design**: Works on desktop and mobile devices

## 🚀 Live Demo

Visit the GitHub Pages site: [https://basmulder03.github.io/qr-file-share/](https://basmulder03.github.io/qr-file-share/)

## 📖 How to Use

### Upload and Share:
1. Open the web application
2. Drag & drop a file or click to browse
3. Click "Generate QR Code"
4. Share the QR code or copy the link
5. Scan the QR code or open the link on another device to download

### Download:
1. Scan the QR code with your device's camera
2. Open the link in your browser
3. Click "Download File" to save the file

## ⚠️ Limitations

- File size limit: 10MB (with automatic compression for files over 100KB)
- Files are encoded in the URL, so very large files may not work well even with compression
- URL shortening requires an internet connection
- Best suited for documents, images, and small files

## 🛠️ Technology Stack

- Pure HTML, CSS, and JavaScript
- QRCode.js library for QR code generation
- Pako library for gzip compression/decompression
- TinyURL API for URL shortening
- Base64 encoding for file data
- GitHub Pages for hosting

## 📝 License

This project is open source and available for anyone to use.

## 🤝 Contributing

Feel free to submit issues or pull requests to improve the application!