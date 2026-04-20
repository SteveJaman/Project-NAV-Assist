# Project-NAV-Assist

**Research framework for real-time assistive navigation.** This project integrates YOLO-based object detection and lightweight Vision-Language Models (VLM) for semantic scene understanding in Mixed Reality (MR). Designed for low-latency indoor hazard detection and spatial guidance.

## 🚀 System Architecture
The system consists of a Python-based Flask server that processes image requests from an MR headset (e.g., Meta Quest 3) or mobile device, performs dual-stage inference, and returns descriptive spatial feedback.

- **Detection:** YOLO-World (Real-time object localization)
- **Description:** FastVLM 0.5B (Semantic scene understanding)
- **Distance Fusion:** Heuristic depth-pitch integration for obstacle proximity estimation.

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/SteveJaman/Project-NAV-Assist.git](https://github.com/SteveJaman/Project-NAV-Assist.git)
   cd Project-NAV-Assist
