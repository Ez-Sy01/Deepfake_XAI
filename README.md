# Deepfake Detection with Explainable AI (XAI)

This repository contains code implementations for applying Explainable AI (XAI) techniques to deepfake detection models.  
We use visualization methods like **Grad-CAM**, **LIME**, and **SHAP** to interpret model decisions.

## 📦 Download Project
You can download the entire project as a ZIP file
-> https://huggingface.co/spaces/Ez-SY01/DF_SW_XAI/resolve/main/DeepSCAN_XAI.zip

## 📂 Project Structure
```
├── gradio
  ├── algorithms/ # Pretrained models or model algorithmss
    ├── FreqNet/ # XAI methods (e.g., GradCAM, LIME, SHAP)
    ├── FreqNet_CAM/ # saved Input Image 
    ├── Grad_FreqNet/ # main Deepfake algorithm
    ├── GradCAM/ # Grad-CAM main code
  ├── SW_GradCAM.py # Script to run GRADCAM
├─ example_fake_image.png
├─ example_real_image.jpg
└── README.md
```
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
-> we do not provide requirements.txt

### 3. Run Grad-CAM by FreqNet
```
python SW_GradCAM.py
```
After running, the local and public links will remain active for one week.

## 📝 Notes
The pretrained model used is based on FreqNet trained on OpenForensics.

All outputs are class-specific explanations (Real vs. Fake).

This is a research prototype — for educational and research use.
