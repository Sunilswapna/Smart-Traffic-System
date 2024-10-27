# Smart Traffic System

## Project Links
1. [Streamlit Webapp](https://omdena-jakarta-traffic-system.streamlit.app/)
2. [Pitch Deck Video](https://clipchamp.com/watch/R69z4mhQp3o)
3. [Omdena Chapter Link](https://omdena.com/chapter-challenges/predicting-road-defects-and-optimizing-traffic-light-countdown-to-reduce-congestion-in-indonesia/)

## Background
**Traffic Management** refers to a combination of measures designed to preserve traffic capacity and improve the security, safety, and reliability of the overall road transport system. These measures utilize ITS (Intelligent Transportation Systems) to optimize road network performance and ensure that:
- Traffic flows smoothly and efficiently.
- Roads are well-maintained and safe for all users, including pedestrians and cyclists.
- Congestion, pollution, and accidents are minimized.
- Vehicles maintain appropriate speeds and follow correct lanes.

## Solution
**This project aims to provide smart solutions to address challenges in traffic management:**

- Vehicle Category Classification and Detection
- Traffic Density Classification
- Pothole Object Detection

| No | Description                            | Dataset | Kaggle Code | Model Weights |
|----|----------------------------------------|---------|-------------|---------------|
| 1  | Vehicle Category Classification and Detection | [Dataset](https://www.kaggle.com/datasets/sakshamjn/vehicle-detection-8-classes-object-detection) | [Notebook](https://www.kaggle.com/code/sudhanshu2198/vehicle-category-object-detection-pytorch) | [Weights](https://www.kaggle.com/datasets/sudhanshu2198/vehicle-categorization-detection-earned-weights) |
| 2  | Traffic Density Classification         | [Dataset](https://www.kaggle.com/datasets/rahat52/traffic-density-singapore) | [Notebook](https://www.kaggle.com/code/sudhanshu2198/traffic-density-classification-using-efficientnet) | [Weights](https://www.kaggle.com/datasets/sudhanshu2198/traffic-density-classification-learned-weights) |
| 3  | Pothole Object Detection               | [Dataset](https://www.kaggle.com/datasets/andrewmvd/pothole-detection) | [Notebook](https://www.kaggle.com/code/sudhanshu2198/real-time-pothole-detection-using-ssd) | [Weights](https://www.kaggle.com/datasets/sudhanshu2198/pothole-detection-learned-weights) |

## 🛠 Skills
Pytorch, Torchvision, Ultralytics, OpenCV, Numpy, Streamlit, Git

## Directory Tree
```bash
├── notebooks
│   ├── real-time-pothole-detection-using-ssd.ipynb
│   ├── traffic-density-classification-using-efficientnet.ipynb
│   └── vehicle-category-object-detection-pytorch.ipynb
├── webapp
│   ├── images
│   │   ├── category_img
│   │   ├── pothole_img
│   │   ├── density_img
│   │   └── home_page
│   ├── pages
│   │   ├── Pothole_Detection.py
│   │   ├── Traffic_Density_Classification.py
│   │   └── Vehicle_Category_Detection.py
│   ├── videos
│   │   ├── raw_clip.mp4
│   │   └── annotated_clip.mp4
│   ├── weights
│   │   ├── pothole_model.pth
│   │   ├── traffic_density.pth
│   │   └── vehicle_categorization.pth
│   ├── Introduction.py
│   ├── utils.py
│   ├── requirements.txt
│   └── packages.txt
├── README.md
├── LICENSE
└── .gitignore

```
# Road Defects Prediction

This project focuses on improving road safety and efficiency through advanced techniques for vehicle classification, traffic density management, and pothole detection. Key modules address vehicle categorization, traffic density classification, and pothole object detection, contributing to overall road management and maintenance.

## Project Features

### 1. Vehicle Category Classification and Detection
Vehicle speed is a critical factor in road safety, with each 1 km/h increase in speed linked to a 3% increase in accident risk. Detecting and categorizing vehicle types in traffic flow supports speed limit enforcement, enhancing road safety.

- **Model Used**: Single Shot Detector (SSD) with MobileNet_v3 backbone  
- **Performance**: Achieved a mean average precision (mAP) of **0.645** on the test dataset at IOU=0.50

### 2. Traffic Density Classification
Effective traffic management is crucial for ensuring smooth, safe transportation. Classifying traffic density helps manage traffic flow during peak hours, optimizing road safety and efficiency.

- **Classification Levels**: Empty, Low, Medium, High, and Jam  
- **Model Used**: EfficientNet_b0  
- **Performance**: Achieved a mean average accuracy of **0.93** on the test dataset

### 3. Pothole Object Detection
Timely road maintenance is essential for safe and efficient travel. Pothole detection aids in early identification of road defects, reducing repair costs and enhancing road quality.

- **Model Used**: Single Shot Detector (SSD) with MobileNet_v3 backbone  
- **Performance**: Achieved a mean average precision (mAP) of **0.512** at IOU=0.50

## Future Development Goals
- Road Lane Instance Segmentation
- License Plate Recognition
- Vehicle Tracking for Speed Measurement

## Running the Web Application Locally

Follow these steps to clone the project repository and run the web application on your local machine.

### Step 1: Clone the Project
```bash
git clone https://github.com/Sunilswapna/Smart-Traffic-System-main
```
### Step 2: Navigate to the Project Directory
```bash
cd Smart-Traffic-System/webapp
```
### Step 3: Create a Virtual Environment and Install Dependencies
On Windows:
```bash
python -m venv venv
source venv/Scripts/activate
pip install -r requirements.txt
```
On macOS/Linux:
```bash
python -m venv venv
source venv/Scripts/activate
pip in
```
### Step 4: Run the Web Application
```bash
streamlit run Introduction.py
```
