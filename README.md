
# SightGuardian

SightGuardian is an innovative 3D spatial visualization platform designed to offer immersive environmental awareness for surveillance and site monitoring. It integrates real-time 3D model rendering, camera feeds, and interactive UI to allow users to view physical spaces in a digital, spatially accurate format.

## 🌐 Why We Need This

Traditional surveillance systems provide flat, 2D camera feeds. These are difficult to spatially interpret, especially in large environments. SightGuardian aims to:

- Map camera feeds onto 3D models for real-time awareness
- Offer immersive, interactive surveillance
- Make situational decisions faster and more accurately

## 🚨 Problem It Solves

- Lack of spatial awareness with standard CCTV
- Delays in emergency response due to non-intuitive views
- Disjointed UI systems and poor integration between maps and feeds

## 🔍 Key Features

- 3D model rendering using WebGL/Three.js
- Real-time camera feed overlays
- Google Maps integration for precise geo-location
- Interactive camera selection and view navigation
- Scalable component-based frontend (React.js)

## 🛠️ Tech Stack

- Frontend: React, Three.js, Google Maps API
- Backend: Node.js, Express (can integrate with OpenCV or similar for analytics)
- Other Tools: WebSocket (for real-time), TailwindCSS

## 🚀 Setup Guide

```bash
git clone https://github.com/your-username/SightGuardian.git
cd SightGuardian
npm install
npm run dev
```

Make sure you add the required `.env` file with:

```
REACT_APP_GOOGLE_MAPS_API_KEY=your_api_key
REACT_APP_BACKEND_URL=http://localhost:5000
```

## 📷 Usage

- Launch the app
- Upload or fetch the 3D model of the monitored site
- Map each camera's RTSP feed to corresponding coordinates
- View live feeds with camera FOV displayed spatially

## 🤝 Contributing

PRs and feedback are welcome. Please read our `CONTRIBUTING.md`.

## 📄 License

MIT License © 2025

## 📚 References

- [Three.js Documentation](https://threejs.org/docs/)
- [Google Maps Geospatial API](https://developers.google.com/maps/documentation/geospatial/overview)
- [WebRTC / RTSP Streams](https://www.videolan.org/)
- Blog: [Why Spatial Surveillance Matters](https://example.com/spatial-awareness-blog)

## 🙌 Made by Azeem Shafeeq

Website: [azeems.netlify.app](https://azeems.netlify.app)  
LinkedIn: [@azeemshafeeq](https://www.linkedin.com/in/azeemshafeeq)
