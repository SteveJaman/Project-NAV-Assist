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
   ```
   
2. **Environment Setup:**
    It is recommended to use Python 3.13.
    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Windows: .venv\Scripts\activate
    pip install -r requirements.txt
   ```
   
3. **Model Weights (Local Only):**
    Due to size constraints, model weights are not included in the repository. Place the following in the FastVLM_Server/ directory:
- yolov8s-worldv2.pt
- llava-fastvithd_0.5b_stage2/

### 🖥️ Running the Server
   ```bash
   python fastvlm_yolo_world.py
   ```
   
Note: The server includes a Windows-specific pathing fix to resolve absolute directory issues in the Transformers library.
### ⚖️ License

Distributed under the MIT License. See LICENSE for more information.
