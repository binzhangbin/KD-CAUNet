# KD-CAUNet
# 🧠 Code Pre-release Statement  

**This repository contains the official implementation for the paper "KD-CAUNet: Geometry-Aware Attentive UNet with Channel-Level Knowledge Distillation for Joint Acoustic Source Range and Depth Estimation in Shallow Water"**  

## 📜 Current Status  
- 🔒 Core code and experimental data are temporarily withheld to ensure data security and privacy  
- 📊 All experimental results in the paper were obtained using the complete implementation in this repository  
- ⚙️ Model architecture details are described in Section 2 (Proposed Method) of the paper

## 📹 Demo
Due to the review process, the full source code will be released
upon acceptance. To demonstrate the effectiveness of our method, we provide a
demo video of our approach running on test data:

<video src="demo.mp4" controls width="100%"></video>

If the video does not play above, you can [download it here](demo.mp4).

## 🚀 Release Plan  
| Stage | Content | Timeline |
|-------|---------|----------|
| Paper Acceptance | Open-source basic framework code | Within 24 hours of acceptance |
| Formal Publication | Release complete training/inference code | Upon paper online publication |
| Supplementary Verification | Public benchmark dataset release | Within 24 hours of publication |

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔍 Future Contents  
```bash
├── data/                             # Dataset
│   ├── hlah/                         # HLAH dataset 
│   ├── hlas/                         # HLAS dataset 
│   ├── vla/                          # VLA dataset 
├── uw_unet/                          # Baseline Backbone 
│   ├── unet_model.py                 
│   └── u_parts.py
├── uw_caunet/                        # CAUNet Backbone 
│   ├── caunet_model.py                 
│   └── cau_parts.py
├── uw_kdcauunet/                     # KD-CAUNet Backbone 
│   ├── kdcaunet_model.py                 
│   └── kdcau_parts.py          
│   ...                               # Other benchmark network models 
├── pretrained_models/                # Pre-trained weights
│   └── hlah_teacher.pth              # SWellEx-96 HLAH model for pretraining
│   └── hlas_teacher.pth              # SWellEx-96 HLAS model for pretraining
│   └── vla_teacher.pth               # SWellEx-96 VLA model for pretraining
├── utils/                            # Utils scripts
│   ├── data_load_utils.py            # Loading data
├─── ...                              # Plot and evaluation methodology: Accurate, RMSE, Distribution, MAE, AIT, Params, ...
└── main_scripts/                     # Testing scripts
│    └── main_train.py                # Main script for measured data (SWellEx-96 HLAH and HLAS and VLA) training
│    └── main_test.py                 # Main script for measured data (SWellEx-96 HLAH and HLAS and VLA) testing
├─── ...                              # Others code


