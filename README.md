# QR File Share 📱

A simple, client-side web application that allows you to share files instantly using QR codes. Upload a file, generate a QR code, and download it on any other device!

## 🌟 Features

- **File Upload**: Drag & drop or click to upload any file
- **QR Code Generation**: Instantly generates a QR code for your file
- **File Compression**: Automatically compresses files larger than 100KB using gzip compression
- **Base64 Encoding**: Files are encoded in base64 and embedded in the URL
- **Multiple QR Codes with Auto-Chaining**: Automatically splits large files across multiple QR codes when needed
  - **Sequential Mode**: QR codes appear one at a time and automatically advance after each scan (recommended)
  - **All Codes Mode**: Display all QR codes at once for manual scanning
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
4. For large files requiring multiple QR codes:
   - **Sequential Mode (Recommended)**: One QR code is displayed at a time. After scanning each code, the next one automatically appears. Keep the sharing page open while scanning.
   - **Show All Codes**: All QR codes are displayed at once. Scan them in order (1 → 2 → 3...).

### Download:
1. **Single QR Code**: Scan the QR code and download the file directly
2. **Multiple QR Codes (Sequential Mode)**:
   - Scan QR code 1 on your receiving device
   - The sharing device automatically displays QR code 2
   - Continue scanning each code as it appears
   - Once all codes are scanned, click "Download File"
3. **Multiple QR Codes (All Codes Mode)**:
   - Scan all QR codes in order (1 → 2 → 3...)
   - The progress is tracked automatically
   - Once all codes are scanned, click "Download File"

## ⚠️ Limitations

- File size limit: 10MB (with automatic compression for files over 100KB)
- Files are encoded in the URL, so very large files may require multiple QR codes
- Large files will be split across multiple QR codes that need to be scanned in order
- Best suited for documents, images, and small files

## 🛠️ Technology Stack

- Pure HTML, CSS, and JavaScript
- QRCode.js library for QR code generation
- Pako library for gzip compression/decompression
- Base64 encoding for file data
- Session storage for multi-part QR code handling
- GitHub Pages for hosting

## 📝 License

This project is open source and available for anyone to use.

## 🤝 Contributing

Feel free to submit issues or pull requests to improve the application!