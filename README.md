# 🌿 Plant Disease Classification using CNN

## Project Overview
Plant Disease Classification using CNN is a deep learning-based project developed to detect and classify plant leaf diseases from images. The model is trained on the **PlantVillage Dataset** from Kaggle containing **38 classes** of healthy and diseased plant leaves.

The project helps farmers and agricultural users identify diseases quickly by uploading leaf images and receiving predictions with confidence scores and precautionary steps. 

- Model tranined on Kaggle(GPU), web app developed and tested on Google Colab

---

## Features
-  Detect plant leaf diseases using image upload
-  Supports **38 plant disease classes**
-  Displays prediction confidence score
-  Provides disease precautionary steps
-  User-friendly Streamlit web application
-  Fast image processing using PIL
-  Integrated Gemini AI (`gemini-1.5-flash`) for enhanced responses

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
**ResNet9 CNN Architecture** 
A lightweight yet powerful 9-layer residual network featuring skip connections, Batch Normalization, and ReLU activations throughout. Trained end-to-end using CrossEntropyLoss and evaluated without gradient computation using torch.no_grad().

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

### Set Up Gemini API Key
1. This app uses Gemini 1.5 Flash to generate disease descriptions and precautionary steps. Get a free API key at Google AI Studio
```export GOOGLE_API_KEY="your_gemini_api_key_here"```

2. Or set it directly in app.py:
```
import google.generativeai as genai
genai.configure(api_key="your_gemini_api_key_here")
```
## Usage
Run Streamlit App Locally on Colab: ```Open http://localhost:8501, upload a leaf image, and get an instant prediction with AI-generated precaution steps!```

## Project Structure
```
Plant-Disease-Classification/
│── app.py
│── model.pth
│── README.md
```

## Future Enhancements
```
1. Deploy on Streamlit Cloud or Hugging Face Spaces for public access
2. Fine-tune on real-world, field-captured leaf images to reduce validation loss gap
3. Add Grad-CAM heatmaps to visually highlight the diseased region on the leaf
4. Experiment with EfficientNet-B4 or Vision Transformer (ViT) for stronger generalization
5. Support multi-language disease advice for farmers in regional languages
6. Add batch upload — analyze multiple leaves in one session
```

## Acknowledgements
```
1. PlantVillage Dataset — Kaggle
2. PyTorch — Deep learning framework
3. Streamlit — Web app framework
4. Google Gemini 1.5 Flash — Generative AI for disease descriptions
```
