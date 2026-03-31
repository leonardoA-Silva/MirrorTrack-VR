# 🪞 MirrorTrack VR
> **Standalone Full-Body Tracking for Meta Quest 3S using Computer Vision and Specular Reflection.**

---

## 📖 Overview
**MirrorTrack VR** is a research and development project focused on solving one of the biggest challenges in standalone Virtual Reality: **lower-body occlusion**. 

Unlike traditional solutions that require expensive external hardware (IMU or IR trackers), MirrorTrack utilizes the physics of **optics (mirrors)** to expand the headset's field of view. By processing the user's reflection, the system enables leg and foot tracking without any additional sensors.

## 🚀 Technical Innovation
For a developer in Brazil, accessing FBT (Full-Body Tracking) hardware is often limited by high import costs. This project demonstrates how **programming logic** and **linear algebra** can overcome physical hardware limitations, making immersive tracking accessible.

### 🛠️ Core Stack
* **Engine:** Unity 2022.3+ (LTS)
* **Language:** C# (.NET)
* **AI/Computer Vision:** MediaPipe / TensorFlow Lite
* **Mathematics:** Specular Reflection Matrices for 3D coordinate inversion.

---

## 📂 Repository Structure
* `Project-Unity/`: Application source code, pose inversion scripts, and Meta SDK integration.
* `Docs/`: Theoretical documentation on matrix calculations and testing results.
* `Research/`: References on latency, sensor precision, and case studies.

## ⚙️ How it Works (The Logic)
1.  **Passthrough Capture:** The system accesses the raw/processed video feed from the Quest 3S cameras.
2.  **Pose Detection:** AI identifies 33 articulation points (Keypoints) within the mirror's reflection.
3.  **Coordinate Inversion:** A C# script applies a mathematical transformation to "unmirror" the motion, aligning the virtual avatar with the user's real-world body.
4.  **Synchronization:** The processed data is fused with native headset tracking (Head & Hands).

---

## 📈 Development Roadmap
- [x] Initial professional repository architecture and documentation.
- [ ] Implementation of the C# pose detection prototype.
- [ ] Automated distance calibration algorithm.
- [ ] Experimental VRChat integration via OSC protocol.

## 👨‍💻 Author
**Leonardo Alves da Silva**
*High School Senior & Full-stack Developer based in Franca, SP - Brazil.*
*Focused on Virtual Reality, UI/UX, and Hardware Maintenance.*

---
This project is part of my technical portfolio for the **Passaporte para o Futuro 2026** program.