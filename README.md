# 🥔 Potato Leaf Disease Detection

This is a full-stack deep learning project that detects potato leaf diseases using Convolutional Neural Networks (CNNs) — with a ReactJS frontend and a FastAPI backend.

## 🔍 Overview

This system helps identify potato plant leaf diseases (like **Early Blight**, **Late Blight**, or **Healthy**) using a trained CNN model. The goal is to assist farmers and agronomists in early disease detection and treatment.

## 🧠 Model

- Built with **TensorFlow / Keras**
- CNN-based image classifier
- Trained on labeled potato leaf datasets
- Outputs predicted class + confidence score

## 🌐 Web Interface

### ✅ Frontend
- Built in **ReactJS**
- Uploads image via `DropzoneArea`
- Calls backend API for prediction
- Shows results with confidence score and class name

### ⚙️ Backend
- Built using **FastAPI**
- Loads `.h5` deep learning model
- Accepts image via POST `/predict` endpoint
- Returns predicted label + confidence


## 🛠️ Tech Stack
| Layer        | Tools                   |
|--------------|--------------------------|
| 🧠 Model      | Python, TensorFlow, Keras |
| 🖥 Frontend   | ReactJS, Material-UI      |
| 🧪 Backend    | FastAPI, Uvicorn          |
| 📦 Communication | Axios (REST API)       |


 Backend Setup
 
 cd api
pip install -r requirements.txt
uvicorn main:app --reload

Frontend Setup

cd frontend
npm install
npm start
REACT_APP_API_URL=http://localhost:8000/predict


Project Structure:
potato-disease-detection/
├── api/             # FastAPI backend
├── saved_models/    # CNN model (.h5)
├── frontend/        # React frontend
├── README.md
└── requirements.txt


