# Deepfake Detection with Explainable AI (XAI)

This repository contains code implementations for applying Explainable AI (XAI) techniques to deepfake detection models.  
We use visualization methods like **Grad-CAM**, **LIME**, and **SHAP** to interpret model decisions.

## 📂 Project Structure
├── models/ # Pretrained models or model definitions
├── xai/ # XAI methods (e.g., GradCAM, LIME, SHAP)
├── examples/ # Example images and XAI visualization outputs
├── utils/ # Utility functions (e.g., preprocessing)
├── run_gradcam.py # Script to run GradCAM
├── run_lime.py # Script to run LIME
├── run_shap.py # Script to run SHAP
└── README.md

## 🧠 Supported XAI Methods

- [x] Grad-CAM  
- [ ] LIME  
- [ ] SHAP  
- [ ] Integrated Gradients (coming soon)

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/deepfake-xai.git
cd deepfake-xai
```
### 2. Install dependencies
```
pip install -r requirements.txt
```
### 3. Run Grad-CAM by FreqNet
```
python run_gradcam.py --image_path examples/fake1.jpg --model_path weights/model.pth
```

📝 Notes
The pretrained model used is based on XceptionNet trained on FaceForensics++.

All outputs are class-specific explanations (Real vs. Fake).

This is a research prototype — for educational and research use.
