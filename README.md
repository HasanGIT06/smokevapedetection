This project applies **YOLOv8 object detection** to identify cigarettes, vapes, people, and smoke from images. The goal is to support automated detection of smoking-related objects in **smoke-free environments**.

---

## ⚙️ Workflow

### 1. Data Preparation
- Combined **7 datasets** containing Cigarette, Person, Smoke, and Vape classes.
- Standardized class labels and split the data into training, validation, and testing sets.
- Final dataset contains **6,980 Cigarette, 6,865 Person, 3,047 Vape, and 1,222 Smoke** annotations.

### 2. Model Training
- Trained a custom **YOLOv8** object detection model.
- Used **512px image size** with GPU acceleration.
- Evaluated model performance using Precision, Recall, mAP, F1-score, and Confusion Matrix.

### 3. Evaluation
- **mAP@50:** 68.2%
- Person detection: **89.99%**
- Vape detection: **80.1%**
- Cigarette detection: **71.11%**
- Smoke detection: **31.6%**

---

## 📊 Results

- Successfully detected **Person, Vape, and Cigarette** with relatively strong performance.
- The model still faces challenges in detecting **Smoke** due to its visual similarity with the background and cigarette objects and its unpredictable shape and translucency due to lighting. 
- Further improvements can be achieved by adding more smoke data and increasing training epochs, and further data collection in order to better balance the classes.

