# KD-CAUNet
# 🧠 Code Pre-release Statement  

**This repository contains the official implementation for the paper "KD-CAUNet: Geometry-Aware Attentive UNet with Channel-Level Knowledge Distillation for Joint Acoustic Source Range and Depth Estimation in Shallow Water"**  

## 📜 Current Status  
- 🔒 Core code and experimental data are temporarily withheld to ensure data security and privacy  
- 📊 All experimental results in the paper were obtained using the complete implementation in this repository  
- ⚙️ Model architecture details are described in Section 2 (Proposed Method) of the paper

## 📹 Demo
Due to the double-blind review process, the full source code will be released
upon acceptance. To demonstrate the effectiveness of our method, we provide a
demo video of our approach running on test data:

<video src="docs/demo.mp4" controls width="100%"></video>

If the video does not play above, you can [download it here](docs/demo.mp4).

## 🚀 Release Plan  
| Stage | Content | Timeline |
|-------|---------|----------|
| Paper Acceptance | Open-source basic framework code | Within 24 hours of acceptance |
| Formal Publication | Release complete training/inference code | Upon paper online publication |
| Supplementary Verification | Public benchmark dataset release | Within 24 hours of publication |

## 🔍 Future Contents  
```bash
├── core_architecture/                 # Backbone 
│   ├── caunet.py                 
│   └── u_parts.py                        
│   ...                                # Other benchmark network models 
├── pretrained_models/                 # Pre-trained weights
│   └── hlah_dsrmstransunet.pth        # SWellEx-96 HLAH model for testing
│   └── hlas_dsrmstransunet.pth        # SWellEx-96 HLAS model for testing
│   └── vla_dsrmstransunet.pth        # SWellEx-96 VLA model for testing
├── training_scripts/                  # Training scripts
│   ├── main_real_train.py             # Main script for measured data (SWellEx-96 HLAH and HLAS and VLA) data training
│   └── utils_load_dataset.py          # Parameters for data loading
└── test_scripts/                      # Testing scripts
│    └── main_real_test.py             # Main script for measured data (SWellEx-96 HLAH and HLAS and VLA) testing
├─── ...                               # Plot and evaluation methodology: Accurate, RMSE, Distribution, stratified K-fold cross-validation
