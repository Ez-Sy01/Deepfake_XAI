# Deepfake Detection with Explainable AI (XAI)

This repository contains code implementations for applying Explainable AI (XAI) techniques to deepfake detection models.  
We use visualization methods like **Grad-CAM**, **LIME**, and **SHAP** to interpret model decisions.

## 📦 Download
You can download the entire project as a ZIP file
-> https://huggingface.co/spaces/Ez-SY01/DF_SW_XAI/resolve/main/DeepSCAN_XAI.zip

## 📂 Project Structure
```
├── gradio
  ├── algorithms/ # Pretrained models or model algorithmss<br>
    ├── FreqNet/ # XAI methods (e.g., GradCAM, LIME, SHAP)<br>
    ├── FreqNet_CAM/ # saved Input Image <br>
    ├── Grad_FreqNet/ # main Deepfake algorithm<br>
    ├── GradCAM/ # Grad-CAM main code<br>
  ├── SW_GradCAM.py # Script to run GRADCAM<br>
├─ example_fake_image.png<br>
├─ example_real_image.jpg<br>
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
python run_gradcam.py --image_path examples/fake1.jpg --model_path weights/model.pth
```

📝 Notes
The pretrained model used is based on XceptionNet trained on FaceForensics++.

All outputs are class-specific explanations (Real vs. Fake).

This is a research prototype — for educational and research use.
