# Edge AI Based Cooperative V2V Communication System (FastLane)

🚗🔗 **FastLane** is an Edge-AI framework for **cooperative Vehicle-to-Vehicle (V2V) communication** and intelligent transportation safety.  
It benchmarks **YOLOv8** (nano and large) against **Deformable DETR** on the **BDD100K dataset**, providing one of the first systematic evaluations of YOLOv8 for autonomous driving perception.  

---

## 📌 Highlights
- **Unified COCO-format pipeline** for fair benchmarking of CNN and transformer-based detectors.  
- **Evaluation Metrics:** Precision, Recall, mAP@0.5, mAP@0.5–0.95, and inference latency.  
- **Simulator-ready outputs** compatible with **CARLA** (urban driving) and **SUMO** (traffic flow).  
- Focus on both **edge efficiency** (YOLOv8-nano) and **accuracy** (YOLOv8-large, Deformable DETR).  

---

## 🏗 System Architecture
FastLane is organized into five functional layers:
1. **Sensor Fusion:** Camera, LiDAR, radar, GPS integration.  
2. **Edge Processing:** YOLOv8 or Deformable DETR for real-time object detection.  
3. **Model Management:** Stores trained models in COCO format for simulator deployment.  
4. **V2V Communication:** Shares hazard alerts via DSRC or C-V2X.  
5. **Decision & Control:** Merges local + shared detections to guide safe maneuvers.  

---

## ⚙️ Installation
```bash
# clone the repository
git clone https://github.com/mmandour22/Edge_AI_Based_Cooperative_V2V_Communication_System_V2.git
cd Edge_AI_Based_Cooperative_V2V_Communication_System_V2

# install dependencies
pip install -r requirements.txt
