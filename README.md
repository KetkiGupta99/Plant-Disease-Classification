# 🌿 Plant Disease Classification using CNN

## Project Overview
Plant Disease Classification using CNN is a deep learning-based project developed to detect and classify plant leaf diseases from images. The model is trained on the **PlantVillage Dataset** from Kaggle containing **38 classes** of healthy and diseased plant leaves.

The project helps farmers and agricultural users identify diseases quickly by uploading leaf images and receiving predictions with confidence scores and precautionary steps.

---

## Features
- ✅ Detect plant leaf diseases using image upload
- ✅ Supports **38 plant disease classes**
- ✅ Displays prediction confidence score
- ✅ Provides disease precautionary steps
- ✅ User-friendly Streamlit web application
- ✅ Fast image processing using PIL
- ✅ Integrated Gemini AI (`gemini-1.5-flash`) for enhanced responses

---

## Technologies Used
- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Torchvision
- PIL (Python Imaging Library)
- Streamlit
- Google Gemini API (`gemini-1.5-flash`)

---

## Dataset
- **Dataset Name:** PlantVillage Dataset
- **Source:** Kaggle
- **Classes:** 38
- **Type:** Image Dataset of healthy and diseased plant leaves

---

## Model Architecture
The model is based on **ResNet9 CNN Architecture**.

### Configuration:
- Activation Function: ReLU
- Loss Function: Cross Entropy Loss
- Gradient Optimization: `no_grad()` used during evaluation
- GPU Training on Kaggle for faster computation

---

## Model Performance
- **Training Accuracy:** 99.2%
- High accuracy achieved using GPU training

---

## Deployment
The model is deployed using **Streamlit** for an interactive web interface.

---

## Application Workflow
1. Upload plant leaf image
2. Image preprocessing using PIL
3. Model predicts disease class
4. Confidence score displayed
5. Gemini AI provides disease explanation & precautions

---

## Project Structure
```
Plant-Disease-Classification/
│── app.py
│── model.pth
│── README.md
```

## Future Enhancements
```
1. Live camera disease detection
2. Multi-language support
3. Mobile app integration
4. Real-time treatment recommendations
5. Disease severity detection
```
│── model.pth
│── requirements.txt
│── README.md
