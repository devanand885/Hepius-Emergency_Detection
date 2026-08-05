# 🛡️ Hepius - AI-Powered Emergency Detection

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen)](https://devanand885.github.io/Hepius/)

> Smart real-time identification of emergency vs non-emergency visual situations using deep learning and computer vision.

## Project Overview

Hepius is an end-to-end computer vision web application that demonstrates real-time emergency detection running directly inside the browser.
The system uses an EfficientNetB3-based deep learning classifier to detect emergency-like visual patterns from webcam streams or uploaded images.

| Class | Description |
|---|---|
| 🚨 Emergency | Distress, panic, pain, or urgent visual cues |
| 🛡️ No Emergency | Neutral, normal, calm, or non-urgent visual cues |

All inference runs locally in the browser with TensorFlow.js, so user images and video feeds never leave the client device, ensuring 100% data privacy.

## Key Highlights

- **Real-Time Webcam Inference**: Live stream classification with periodic frame predictions
- **Image Upload Analysis**: Upload and analyze single image frames instantly
- **100% Client-Side Privacy**: Runs locally using TensorFlow.js graph model execution
- **Dynamic Interactive Dashboard**: Real-time confidence gauge, score breakdown, and visual alert states
- **GitHub Pages Ready**: Optimized static-host deployment architecture

## Features

- Camera mode with automatic periodic predictions
- Single-image upload and analysis workflow
- Emergency / Non-emergency confidence score visualization
- Visual alert state triggers for high-risk predictions
- Full control to reset/clear camera streams and upload flows
- Responsive, modern glassmorphic dashboard UI

## Model Details

| Property | Value |
|---|---|
| Base Model Architecture | EfficientNetB3 |
| Runtime Format | TensorFlow.js Graph Model |
| Input Shape | 300 x 300 x 3 (RGB) |
| Output | 2-class softmax (Emergency / No Emergency) |
| Inference Engine | TensorFlow.js 4.x (browser runtime) |

## Technical Stack

### Machine Learning
- **Framework**: TensorFlow / Keras
- **Deployment Runtime**: TensorFlow.js 4.x
- **Model Type**: EfficientNetB3-based image classifier

### Web Application
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Icons & Styling**: Font Awesome 6, Google Fonts (Outfit, Space Mono)
- **Visualization**: Custom SVG dashboard gauges & dynamic bar charts
- **Hosting**: GitHub Pages

## Project Structure

```text
Hepius/
├── README.md
├── index.html
├── css/
│   └── styles.css
├── js/
│   ├── main.js
│   ├── model.js
│   ├── ui.js
│   └── charts.js
└── tfjs_graph_model/
    ├── model.json
    └── group1-shard1of12.bin ... group1-shard12of12.bin
```

## Quick Start

### 1) Clone the Repository

```bash
git clone https://github.com/devanand885/Hepius.git
cd Hepius
```

### 2) Run Locally

Run a simple local HTTP server:

```bash
python -m http.server 8000
```

Open your browser at:
`http://127.0.0.1:8000`

### 3) Test the App

1. Click **Start Camera** to test live webcam predictions.
2. Or switch to **Upload** mode to select and analyze an image file.
3. Observe real-time confidence metrics and visual status alerts.

## Author & Contact

**Devanand**

- **GitHub**: [github.com/devanand885](https://github.com/devanand885)
- **Email**: [g.devanand005@gmail.com](mailto:g.devanand005@gmail.com)

If this project helped you, consider giving it a ⭐️ star on GitHub!
