# 🩺 Low-Dose PET Image Enhancement System using U-Net

## 📌 Project Overview

This project presents a deep learning-based system for enhancing low-dose Positron Emission Tomography (PET) images using the U-Net architecture.

Reducing radiation dose during PET scans improves patient safety but introduces significant image noise and loss of diagnostic information. This project aims to restore image quality by training a U-Net model to convert low-dose PET images into high-quality enhanced PET images.

This project was developed as a Capstone Project for the Integrated M.Tech in Software Engineering program.

---

## 🎯 Objectives

- Improve the quality of low-dose PET images.
- Reduce image noise while preserving anatomical structures.
- Train a U-Net deep learning model for PET image enhancement.
- Evaluate image quality using PSNR, SSIM, RMSE, and NRMSE.
- Develop a web-based system for PET image enhancement (future work).

---

## 🧠 Model Used

- U-Net (Encoder–Decoder Architecture)
- Framework: PyTorch

---

## 🗂 Dataset

Dataset Source:

Kaggle PET Image Dataset

Images are stored in DICOM (.dcm) format.

Since paired low-dose and high-dose PET datasets were unavailable, synthetic low-dose PET images were generated using Poisson noise from normal-dose PET images.

---

## 🛠 Technologies Used

- Python
- PyTorch
- MONAI
- NumPy
- Matplotlib
- Scikit-Learn
- Pydicom
- Kaggle Notebook

---

## ⚙ Workflow

```

PET Dataset

↓

Read DICOM Images

↓

Image Normalization

↓

Generate Synthetic Low-Dose PET

↓

Train U-Net Model

↓

Validate Model

↓

Test Model

↓

Generate Enhanced PET Image

↓

Evaluate Results

```

---

## 📊 Evaluation Metrics

The model is evaluated using:

- PSNR (Peak Signal-to-Noise Ratio)
- SSIM (Structural Similarity Index)
- RMSE (Root Mean Square Error)
- NRMSE (Normalized RMSE)

---

## 📈 Sample Training Results

| Metric | Value |
|---------|-------|
| Training Epochs | 50 |
| Best Validation Loss | 0.00143 |
| PSNR | ~44 dB |
| SSIM | ~0.994 |

---

## 📂 Project Structure

```

Low-Dose-PET-Image-Enhancement-System/

│

├── adithya-unet-pet.ipynb

├── README.md

├── best_unet_pet.pth

├── requirements.txt

└── sample_outputs/

```

---

## 🚀 How to Run

1. Clone the repository

```

git clone https://github.com/adithyaruthvik7777-commits/-Low-Dose-PET-Image-Enhancement-System-.git

```

2. Install dependencies

```

pip install -r requirements.txt

```

3. Open the notebook

```

adithya-unet-pet.ipynb

```

4. Run all notebook cells.

---

## 📌 Future Improvements

- Develop a Flask-based web application.
- Support real-time PET image enhancement.
- Compare U-Net with Restormer and SwinIR.
- Train on real paired low-dose PET datasets.
- Deploy the application on Render or Hugging Face Spaces.

---

## 👨‍💻 Author

**P. S. Adithya Ruthvik**

Integrated M.Tech in Software Engineering

VIT-AP University

GitHub:
https://github.com/adithyaruthvik7777-commits

---

## 📜 License

This project is developed for educational and research purposes.
