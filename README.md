# 🚨 SightGuardian: AI-Powered Smart Surveillance System

![Banner](./assets/sightguardian-banner.png)
*Detect. Analyze. Protect. — Real-time smart surveillance made practical with Hugging Face models.*

---

## 📌 Overview

**SightGuardian** is an AI-driven surveillance assistant designed to detect and report suspicious behavior, safety hazards, or emergency events from real-time video streams.

This project uses cutting-edge models from [Hugging Face](https://huggingface.co/) to intelligently process video feeds, identify abnormal activities (e.g., fights, fire, weapons), and deliver actionable alerts — all while preserving privacy and enabling scalability.

---

## 💡 Key Features

* 🎯 Real-time **object detection** (e.g., people, weapons, smoke)
* 🧠 **Anomaly detection** for violence, loitering, or falls
* 🔥 Fire & smoke detection using **image classification**
* 📝 Auto-generated **incident reports** using text generation
* 📍 **Location-aware** tracking with map-based dashboards
* ⚠️ Alerting system with webhooks, email, or SMS
* 🛡️ Privacy-first: no facial recognition, edge-processing support
* 🌐 Scalable architecture (cloud or on-prem)

---

## 🔍 Use Cases

* City surveillance & smart city initiatives
* Public event crowd monitoring
* Retail and warehouse security
* School & campus safety enforcement

---

## 🧠 AI Tasks Used (from Hugging Face)

| Task                        | Purpose                                             |
| --------------------------- | --------------------------------------------------- |
| `Object Detection`          | Identify threats like weapons or suspicious objects |
| `Video Classification`      | Detect violent or unusual behavior                  |
| `Image Segmentation`        | Extract people/objects from background              |
| `Text Generation`           | Summarize detected events                           |
| `Visual Question Answering` | Ask questions like “is someone lying down?”         |
| `Depth Estimation`          | Estimate distance between entities                  |
| `Image-to-Text`             | Describe scenes for auto-reporting                  |

---

## 🧰 Tech Stack

### Frontend

* [Next.js](https://nextjs.org/)
* [Tailwind CSS](https://tailwindcss.com/)
* [Mapbox](https://www.mapbox.com/) / Google Maps API
* [Socket.IO](https://socket.io/) for live alert streaming

### Backend

* [FastAPI](https://fastapi.tiangolo.com/)
* [PostgreSQL](https://www.postgresql.org/) + PostGIS
* [Redis](https://redis.io/) for task queuing
* [OpenCV](https://opencv.org/) + [FFmpeg](https://ffmpeg.org/) for video processing

### AI/ML

* [Transformers](https://huggingface.co/transformers/)
* [PyTorch](https://pytorch.org/)
* [ONNX Runtime](https://onnxruntime.ai/)
* [YOLOv7](https://github.com/WongKinYiu/yolov7) or Hugging Face vision models

---

## 🖼️ System Architecture

```
[Camera Stream or RTSP Feed]
      ↓
[Video Preprocessor (OpenCV/FFmpeg)]
      ↓
[Inference Engine (Object Detection, Anomaly, Segmentation)]
      ↓
[Alert Scorer & Event Aggregator]
      ↓
[PostgreSQL + Redis Queue]
      ↓                   ↓
[Incident Report Engine]  [Alert Notifier]
      ↓                   ↓
[Frontend Dashboard (Map + Timeline + Viewer)]
```

---

## 📸 Screenshots (Mockups)

> Replace with real screenshots once implemented

| Live Detection              | Incident Timeline          | Report Example           |
| --------------------------- | -------------------------- | ------------------------ |
| ![](./assets/live-feed.png) | ![](./assets/timeline.png) | ![](./assets/report.png) |

---

## ⚙️ Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/sightguardian.git
cd sightguardian
```

### 2. Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload
```

### 3. Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### 4. Start Camera Feed (for testing)

```bash
ffmpeg -i test-video.mp4 -f image2pipe -vcodec rawvideo -pix_fmt rgb24 -
```

---

## 🧪 Sample Data Sources

* Public camera feeds: [https://trafficcams.com/](https://trafficcams.com/)
* Drone data: [OpenAerialMap](https://openaerialmap.org/)
* Video datasets: [UCF-Crime](http://crimelab.cs.ucf.edu/), [VIRAT Video](https://viratdata.org/)

---

## 🚀 Roadmap

* [x] Object detection (people, weapons, fire)
* [x] Incident report generation
* [ ] Real-time video streaming from edge devices
* [ ] Activity recognition (e.g., falls, fights)
* [ ] VQA module integration
* [ ] Admin dashboard with permissions
* [ ] Docker + Kubernetes deployment support

---

## 🛡️ Ethical & Privacy Principles

* 🚫 No facial recognition used
* ✅ Edge inference supported to avoid cloud video uploads
* 📜 Transparent logging and data retention policies
* 👮 Human-in-the-loop alerts for critical events

---

## 📈 Performance Goals

| Metric              | Target  |
| ------------------- | ------- |
| Detection Accuracy  | ≥ 85%   |
| False Positive Rate | ≤ 10%   |
| Report Latency      | ≤ 3 sec |
| Stream Delay        | ≤ 2 sec |

---

## 🤝 Contributing

1. Fork the repo and clone it locally.
2. Create a new branch: `feat/your-feature-name`.
3. Make your changes and commit: `git commit -m 'feat: added new feature'`
4. Push to the branch: `git push origin feat/your-feature-name`
5. Open a pull request!

---

## 📄 License

[MIT](LICENSE)

---

## 💬 Contact

Built by [Your Name](https://yourwebsite.com)
🔗 LinkedIn · 💼 Portfolio · ✉️ [azeemshafeeq125@gmail.com](mailto:azeemshafeeq125@gmail.com)

---

## ⭐️ Show Your Support

If you like this project, please give it a ⭐️ and share it with others!

