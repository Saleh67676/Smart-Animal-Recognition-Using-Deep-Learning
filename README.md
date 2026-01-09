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

###2️⃣ Dataset Setup
Make sure your dataset is organized like this:

bash
Copy code
animals/
 ├── cat/
 ├── dog/
 ├── bat/
 ├── deer/
 ├── bear/
 └── ...
Each subfolder represents one animal class.
All images should be in .jpg format.

###3️⃣ Training the Model
Run the training script or notebook.
The model will:

Load and preprocess images

Freeze MobileNetV2 base layers

Train for 15 epochs

Save the final model as:

Copy code
animal_cnn.keras


###4️⃣ Testing & Inference
The testing script:

Randomly selects an image from the dataset

Applies preprocessing

Uses the trained model to predict the class

A window will display the image with its predicted label, for example:

makefile
Copy code
Prediction: badger

```bash
