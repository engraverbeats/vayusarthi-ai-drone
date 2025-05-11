# 🚁 VayuSarthi – AI-Powered Emergency Response Drone

**VayuSarthi** is an AI-powered drone system designed for rapid response in medical emergencies, disaster zones, and public safety scenarios. Developed under the SIH problem statement ID 1533, it integrates autonomous navigation, real-time tracking, and aid delivery using onboard AI and robust hardware.

---

## 🌟 Key Features

- **Autonomous Navigation**: GPS-guided flight with Pixhawk + ArduPilot
- **AI-Based Detection**: Real-time object and human tracking using TensorFlow, OpenCV, and MediaPipe
- **LIDAR + Vision**: Enhanced environment perception for obstacle avoidance
- **Live Video Streaming**: Via Quectel RG50xQ 4G/5G communication module
- **Aid Deployment**: Delivers medical/food supplies using servo-controlled payload systems
- **Control Room Command**: Remote command with emergency override (e.g., tear gas or ink spray)
- **Scalable**: Supports multi-drone deployment for large-scale rescue operations

---

## 🧠 Tech Stack

- **AI Frameworks**: TensorFlow, MediaPipe, OpenCV
- **Hardware**: Raspberry Pi, Pixhawk, LIDAR, GPS, Camera
- **Communication**: Quectel RG50xQ (5G/4G), MAVLink
- **Software**: ROS, ArduPilot, Mission Planner
- **Object Models**: YOLOv5, Custom-trained models

---

## 📂 Project Structure

```
vayusarthi-ai-drone/
├── src/                        # Python scripts for drone control and AI
├── models/                     # ONNX / TensorRT AI models
├── hardware_specs/            # Hardware setup guides
├── config/                    # ROS/launch configurations
├── docs/                      # Documentation and README
├── requirements.txt
├── CMakeLists.txt
├── package.xml
└── .gitignore
```

---

## 🚀 Getting Started

1. Clone the repo and install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Launch the ROS mission:
   ```bash
   roslaunch config/flight_mission.launch
   ```

3. Run object tracking manually:
   ```bash
   python src/object_tracking.py
   ```

---

## 🎥 Demo / References

- [Dojo for Drones – Jetson Nano Setup](https://dojofordrones.com/jetson-nano-drone/)
- [Quectel RG50xQ Series Datasheet](https://www.quectel.com/product/5g-rg50xq/)
- [YOLO Object Detection Blog](https://www.v7labs.com/blog/yolo-object-detection)

---

## 👨‍💻 Contributors
- Ayush Ranjan (AI & Drone Systems)
- Team VayuSarthi – SIH 2024 Public Safety Category

---

## 📜 License

MIT License
