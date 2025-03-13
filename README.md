# 🏙️ Vacant Land Detection using YOLOv8  

## 🚧 Project Status: In Progress  
This project is currently under development. Some features and results may change as improvements are made. Contributions and feedback are welcome 

## 📌 Project Description  
This project aims to detect vacant lands in Casablanca using **YOLOv8**. The goal is to generate a geospatial map highlighting these vacant lands, which can be used for urban planning, real estate analysis, and development strategies.  

## 🚀 Objectives  
- Train a **YOLOv8** model to detect vacant lands from aerial/satellite images.  
- Generate a **map** displaying the detected areas.  
- Improve detection accuracy using geospatial and machine learning techniques.  

## 🛠️ Prerequisites  
Ensure you have the following dependencies installed before running the project:  

```bash
pip install ultralytics opencv-python numpy geopandas shapely matplotlib
```

## 📂 Project Structure  
```
vacant-land-detection-yolo/
├── data/               # Dataset (images, annotations, etc.)
├── models/             # YOLOv8 trained models
├── scripts/            # Python scripts for training, inference, and mapping
├── results/            # Detected areas & generated maps
├── notebooks/          # Jupyter Notebooks for model training and evaluation
├── README.md           # Project documentation
├── requirements.txt    # List of dependencies
├── .gitignore          # Files to ignore in Git
```

## 🔥 How to Run  
1. **Clone this repository:**  
   ```bash
   git clone https://github.com/YOUR_USERNAME/vacant-land-detection-yolo.git
   cd vacant-land-detection-yolo
   ```  
2. **Install dependencies:**  
   ```bash
   pip install -r requirements.txt
   ```  
3. **Train the YOLOv8 model (if needed):**  
   ```bash
   yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=50 imgsz=640
   ```  
4. **Run inference on images:**  
   ```bash
   yolo task=detect mode=predict model=models/best.pt source=data/test_images/ save=True
   ```  
5. **(Optional) Convert detections into a geospatial map using `geopandas`.**

## 📊 Expected Results  
- A **trained YOLOv8 model** capable of detecting vacant lands.  
- A **visualization map** showing detected areas in Casablanca.  
- Insights for urban development and planning.  

## 🧪 Model Performance Evaluation  
- **Precision & Recall Metrics:** Evaluate how well the model detects vacant lands.  
- **IoU (Intersection over Union):** Measure detection accuracy.  
- **Confusion Matrix:** Analyze false positives and false negatives.  

## 📌 Technologies Used  
- **YOLOv8** for object detection.  
- **Python** for data processing & modeling.  
- **GeoPandas** & **Shapely** for spatial data analysis.  
- **OpenCV** for image manipulation.  
- **Matplotlib & Folium** for data visualization.  

## 🚀 Future Improvements  
- Increase dataset size for better accuracy.  
- Implement active learning to refine model predictions.  
- Integrate with GIS tools for real-time mapping.  
  

---  

