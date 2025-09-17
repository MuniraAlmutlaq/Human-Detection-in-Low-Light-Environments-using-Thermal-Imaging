# 🔦 Human Detection in Low Light Environments using Thermal Imaging  

## 📌 Project Overview  
This project tackles the challenge of detecting humans in **low-light or night-time environments** using **thermal imaging**. Unlike standard cameras, thermal sensors capture **infrared heat signatures**, making them effective for surveillance, safety, and rescue scenarios where visible light is limited.  

A publicly available **thermal dataset** (originally in YOLO format) was used. The dataset underwent preprocessing steps such as:  
- 🖼️ Resizing  
- 🌗 Brightness adjustment  
- 🧹 Noise filtering  
- 🔄 Annotation conversion to **COCO format** for compatibility  

The goal is to evaluate different **object detection models** and identify the most effective architecture for accurate human detection in thermal images.  

---

## ⚙️ Models Implemented  
The following object detection models were trained and evaluated on the dataset:  

1. 🟢 **YOLOv8n**  
2. 🔵 **YOLOv8s**  
3. 🟠 **Faster R-CNN**  
4. 🟣 **RetinaNet**  

---

## 📊 Evaluation Metrics  
Each model was assessed using standard object detection benchmarks:  

- **mAP@0.5:0.95**  
- **mAP@0.5**  
- **Precision**  
- **Recall**  

These metrics helped compare model performance and robustness under thermal imaging conditions.  

---

## 🚀 Results  
- The comparative evaluation highlighted trade-offs between **accuracy**, **speed**, and **complexity**.  
- YOLOv8 variants showed strong performance in **real-time inference**, while **Faster R-CNN** and **RetinaNet** provided higher **detection precision** in some scenarios.  
- Findings support the adoption of thermal-based detection systems for **night surveillance** and **safety-critical applications**.  

---

## 🛠️ Tech Stack  
- **Python** 🐍  
- **PyTorch**  
- **YOLOv8 (Ultralytics)**  
- **Detectron2 / Torchvision Models**  
- **OpenCV**  
- **COCO & YOLO format handling tools**  
