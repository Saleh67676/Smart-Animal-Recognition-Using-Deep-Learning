# 🐾 Smart Animal Recognition Using Deep Learning

## 📖 Project Overview
This project is an automated system designed to recognize and classify animal species using Deep Learning techniques.  
It leverages **Transfer Learning** with the **MobileNetV2** architecture to achieve high performance in identifying **90 different animal classes**.

---

## 👥 Team Members (Group 6)

- **Hisham Abdullah Almalki**  
- **Saleh Mohammed Alsulami**  
- **Adel Mohammed Alzahrani**  
- **Ali Abdullah Almufarriji**  
- **Omar Alhassan Almaashi**

---

## 🛠️ Tech Stack

- **Framework:** TensorFlow / Keras  
- **Base Model:** MobileNetV2 (Pre-trained on ImageNet)  
- **Libraries:** NumPy, Matplotlib  
- **Optimizer:** Adam Optimizer (learning rate = 1e-3)

---

## 📊 Dataset & Training Details

- **Total Classes:** 90 different animal categories (e.g., antelope, badger, bear, cat, dog, etc.)  
- **Training Set:** 4,320 images  
- **Validation Set:** 1,080 images  
- **Image Size:** 224 × 224 pixels  
- **Data Augmentation:**
  - Rotation: 20°
  - Zoom: 0.2
  - Horizontal Flip  

- **Results:**
  - Training Accuracy ≈ **96.7%**
  - Validation Accuracy ≈ **87.6%** (after 15 epochs)

---

## 🚀 How to Run

### 1️⃣ Prerequisites
Install the required libraries:

pip install numpy tensorflow matplotlib

---
2️⃣ Dataset SetupMake sure your dataset is organized like this:Plaintextanimals/
 ├── cat/
 ├── dog/
 ├── bat/
 ├── deer/
 ├── bear/
 └── ...
Each subfolder represents one animal class1.All images should be in .jpg format22.+13️⃣ Training the ModelRun the training script or notebook (llm.ipynb). The model will:Preprocess: Resize images to $224 \times 224$3333.+1Freeze Layers: Use MobileNetV2 with frozen base layers4444.+1Train: Execute the training process for 15 epochs5555.+1Save: Export the final model as animal_cnn.keras6.4️⃣ Testing & InferenceThe testing script will:Random Selection: Pick a random image from the dataset7777.+1Predict: Use the trained model to predict the animal class8.Visualize: Display the image with its predicted label (e.g., Prediction: badger)9999

```bash
