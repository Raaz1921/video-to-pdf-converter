# 📹 Video to PDF Converter (Browser-Based)

A **browser-based Video to PDF Converter** that converts videos into **screenshot-based PDFs** using **fixed time intervals** or **smart scene detection** — fully **client-side**, with **no backend**, **no uploads**, and **no server cost**.

> ✅ Runs entirely in your browser  
> ✅ Works offline after loading  
 

---

## 🔍 What is Video to PDF?# 📹 Video to PDF Converter 

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![jsPDF](https://img.shields.io/badge/jsPDF-2.5.1-red?style=flat)](https://github.com/parallax/jsPDF)

A **browser-based Video to PDF Converter** that transforms videos into **screenshot-based PDFs** using **fixed time intervals** or **smart scene detection**. Runs entirely **client-side** with **no backend**, **no uploads**, and **no server costs**.

![Video to PDF Demo](https://img.shields.io/badge/Demo-Live-brightgreen)

---

## 🔍 What is Video to PDF?

**Video to PDF** means extracting visual frames (screenshots) from a video and compiling them into a multi-page PDF document. Each page represents a meaningful moment in the video — slides, scenes, or key frames.

This project does exactly that — **locally in your browser**, with no server required.

---

## ✨ Features

### Core Functionality
- 📁 **Local Video Upload** - Support for MP4, WebM, and more
- 🖼️ **Frame to PDF Conversion** - Converts video frames into PDF pages
- ⏱️ **Fixed Interval Capture** - Capture screenshots at regular time intervals
- 🎬 **Smart Scene Detection** - Automatically detect scene changes
- 🔒 **Max Gap Protection** - Prevents long gaps in scene detection mode
- ✏️ **Custom PDF Naming** - User-defined PDF filenames 

### User Experience
- 🧾 **Multi-page PDF Generation** - Create comprehensive video summaries
- 📊 **Real-time Progress Bar** - Track conversion progress
- 🖼️ **Live Preview Grid** - Preview all captured screenshots before PDF generation
- 🌙 **Dark Mode** - Eye-friendly dark theme
- 📱 **Responsive Design** - Works on desktop and mobile devices

### Privacy & Performance
- 🔐 **100% Client-Side** - No uploads, no tracking, no data collection
- ⚡ **Optimized Processing** - Sequential image loading prevents browser freezing
- 💾 **Memory Efficient** - Smart resource management
- 🌐 **Works Offline** - Functions without internet after initial load

---

## 🚀 Quick Start

### Option 1: Direct Use
1. Download the `Index.html` file
2. Open it in any modern web browser (Chrome, Firefox, Edge, Safari)
3. Start converting videos!

### Option 2: Local Development
```bash
# Clone the repository
git clone https://github.com/yourusername/video-to-pdf-converter.git

# Navigate to the directory
cd video-to-pdf-converter

# Open in browser
open Index.html  # macOS
start Index.html # Windows
open Index.html  # Smartphone (Chrome)
xdg-open Index.html # Linux
```

No dependencies to install, no build process needed!

---

## 📖 How to Use

### 1. Upload Your Video
- Click **"Choose Video File"**
- Select a video from your device
- Preview appears automatically

### 2. Configure Settings

#### **Mode Selection**
Choose between two capture modes:

**⏱️ Fixed Interval Mode**
- Captures screenshots at regular time intervals
- Perfect for presentations, lectures, tutorials
- Example: Capture every 5 seconds

**🎬 Scene Detection Mode**
- Automatically detects when scenes change
- Prevents gaps with max-gap protection
- Ideal for dynamic content like movies, gameplay

#### **Time Range** (Optional)
- Set **Start Time** and **End Time** to convert specific portions
- Great for extracting highlights

#### **Advanced Options**
- **Screenshot Interval**: Time between captures (Fixed Interval mode)
- **Check Interval**: How often to check for scene changes
- **Max Gap**: Maximum time between forced captures
- **Sensitivity**: Scene detection sensitivity (Low/Medium/High)

### 3. Generate PDF
1. Click **"Generate PDF"**
2. Watch the progress bar
3. Preview all captured screenshots
4. Enter your desired filename when prompted
5. PDF downloads automatically!

---

## 🛠️ Technical Details

### Technology Stack
- **HTML5** - Structure and video handling
- **CSS3** - Responsive design with dark mode
- **Vanilla JavaScript** - Core logic and processing
- **jsPDF 2.5.1** - PDF generation
- **Canvas API** - Frame extraction
- **HTML5 Video API** - Video manipulation

### Browser Compatibility
- ✅ Chrome/Edge (Recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera
  

### Key Algorithms

**Scene Detection Algorithm**
```
For each frame:
  1. Extract image data using Canvas API
  2. Compare with previous frame (pixel difference)
  3. If difference > threshold → Scene change detected
  4. If time since last capture > max gap → Force capture
  5. Generate preview thumbnail
```

---

## 📂 Project Structure

```
video-to-pdf-converter/
├── Index.html          # Main application file (standalone)
└── README.md          # This file
```

**Single File Architecture**: Everything is contained in one HTML file for maximum portability and ease of use.

---

## 🎯 Use Cases

- **📚 Educational**: Convert lecture videos to study PDFs
- **🎓 Presentations**: Extract slides from recorded presentations
- **🎮 Gaming**: Create gameplay moment collections
- **🎬 Movies/Videos**: Generate scene summaries
- **📺 Tutorials**: Create step-by-step visual guides
- **📊 Webinars**: Document important moments

---

## ⚙️ Configuration Options

### Fixed Interval Mode
| Setting | Default | Description |
|---------|---------|-------------|
| Screenshot Interval | 5s | Time between captures |
| Start Time | 0s | Video start point |
| End Time | Video end | Video end point |

### Scene Detection Mode
| Setting | Default | Description |
|---------|---------|-------------|
| Check Interval | 10s | How often to check for changes |
| Max Gap | 60s | Maximum time without capture |
| Sensitivity | 25% | Scene change detection threshold |
| Start Time | 0s | Video start point |
| End Time | Video end | Video end point |

---

## 🔒 Privacy & Security

- ✅ **Zero Data Collection** - Nothing is sent to any server
- ✅ **Local Processing** - All operations happen in your browser
- ✅ **No Tracking** - No analytics, cookies, or user tracking
- ✅ **Open Source** - Fully transparent code
- ✅ **Offline Capable** - Works without internet connection

---

## 🚧 Future Enhancements

- [ ] Batch processing multiple videos
- [ ] Custom PDF page dimensions
- [ ] Image quality settings
- [ ] OCR text extraction
- [ ] Annotation capabilities
- [ ] Cloud storage integration (optional)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).


---

## 🙏 Acknowledgments

- [jsPDF](https://github.com/parallax/jsPDF) - PDF generation library
- HTML5 Canvas API - Frame extraction
- Modern browser developers for powerful web APIs

---

## ⭐ Show Your Support

If you find this project helpful, please consider giving it a ⭐ on GitHub!

---

**Made with 💜 for the open-source community**

**Video to PDF** means extracting visual frames (screenshots) from a video and compiling them into a multi-page PDF document.

Each page represents a meaningful moment in the video (slides, scenes, key frames).

This project does exactly that — **locally in your browser**.

---

## 👨‍💻 Author

Created by [Raaz]


