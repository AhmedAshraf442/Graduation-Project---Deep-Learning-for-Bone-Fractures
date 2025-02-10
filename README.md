# **FracScan - AI-Powered Bone Fracture Detection**

![FracScan Logo](https://github.com/AhmedAshraf442/Graduation-Project---Deep-Learning-for-Bone-Fractures/blob/49cdda28938bd08e4fd48b68b99a3c6c4b567980/Screenshot%202025-02-10%20144700.png)

## **Overview**
FracScan is a deep learning-based system for detecting and classifying bone fractures from X-ray images. It leverages state-of-the-art CNN models such as **ResNet-152, InceptionV3, EfficientNetB1/B5/B6, and YOLOv8** to provide accurate fracture detection and severity classification.

## **Features**
✅ **Fracture Detection:** Identify fractures in X-ray images with high accuracy.  
✅ **Multi-Label Classification:** Classify bone type and abnormality in one model.  
✅ **Explainable AI (XAI):** Uses LIME to visualize model predictions.  
✅ **User-Friendly Interface:** A web-based system built with Django and Flask.  
✅ **API Integration:** Offers a RESTful API for easy integration.

## **Datasets Used**
- **[MURA](https://stanfordmlgroup.github.io/competitions/mura/):** 40,561 X-ray images labeled by radiologists.  
- **[VinDr-SpineXR](https://physionet.org/content/vindr-spinexr/1.0.0/):** 10,466 spine X-ray images with seven abnormality types.  
- **[GRAZPEDWRI-DX](https://figshare.com/articles/dataset/GRAZPEDWRI-DX/14825193):** Pediatric wrist fracture dataset.  
- **FracAtlas:** 4,083 annotated X-ray images for classification and localization.

## **Installation & Usage**
### **Prerequisites**
Ensure you have the following installed:  
- Python 3.x  
- TensorFlow, Keras, OpenCV  
- Flask & Django for backend  
- YOLOv8 for object detection  

### **Installation**
Clone the repository:  
```bash
git clone https://github.com/your_username/FracScan.git  
cd FracScan
```
Install dependencies:  
```bash
pip install -r requirements.txt
```
### **Running the Model**
1. **Preprocess Dataset**  
   ```bash
   python preprocess.py
   ```
2. **Train the Model**  
   ```bash
   python train.py --epochs 50 --batch 16
   ```
3. **Run Inference on an X-ray Image**  
   ```bash
   python inference.py --image path/to/xray.jpg
   ```

## **Results**
📊 **Model Performance:**  
| Model          | Accuracy (%) | Dataset |  
|---------------|------------|---------|  
| EfficientNet-B5 | 93%        | MURA + LERA |  
| ResNet-152     | 67%        | VinDr-SpineXR |  
| EfficientNet-B6 | 96%        | Bone Fracture Type |  
| YOLOv8-L       | 58 mAP     | GRAZPEDWRI-DX |  

## **Deployment**
FracScan offers a web-based interface where users can upload X-ray images and receive real-time fracture analysis. The system is built using **Django (backend), Flask (API), and TensorFlow (model inference).**  

## **Authors**
Developed by a team of AI engineers from Cairo University.  

## **License**
This project is licensed under the **MIT License**.

