🎯 Sack Bag Counting System (Computer Vision Analytics)
📌 Problem Statement
Build a computer vision system to automatically detect, track, and count sack bags from video streams.

---

🚀 Solution Overview
This system uses a complete AI video analytics pipeline:

- Object Detection → YOLOv8
- Multi-Object Tracking → ByteTrack
- Counting Logic → Line Crossing Algorithm
- Analytics Output → Processed Video + Count

🧠 System Architecture

Video Input  
↓  
YOLOv8 Object Detection  
↓  
ROI Filtering (Domain Logic)  
↓  
Multi-Object Tracking (ByteTrack)  
↓  
Unique ID Assignment  
↓  
Virtual Line Crossing  
↓  
Bag Count Output + Analytics Video  



 Tech Stack
- Python
- OpenCV
- YOLOv8 (Ultralytics)
- ByteTrack
- Google Colab
- NumPy



⚙️ Pipeline Components

1. Detection
YOLOv8 detects sack bags in each frame.

 2. Tracking
ByteTrack assigns persistent IDs to each detected bag.

 3. Counting
A virtual line is defined.  
Each unique ID crossing the line is counted once.

 🎥 Output
- Annotated video with:
  - Bounding boxes
  - Tracking IDs
  - Counting line
  - Live counter
- Final bag count printed in console

 📈 Features
- Real-time processing
- No duplicate counting
- Robust tracking
- ROI-based filtering
- Production-grade pipeline

