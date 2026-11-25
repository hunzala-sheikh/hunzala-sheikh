# Hi, I'm Hunzala 👋

**Computer Vision and Medical Imaging Engineer.** I train deep-learning models that recognise and outline structures in
medical and microscopy images, and I ship them as working tools that clinicians and researchers can actually use.

- 🔬 Segmentation and instance segmentation for **microscopy, embryology and MRI**
- 🏷️ Training on **real-world labels**: small expert-annotated sets, noisy reports, weak supervision
- 📏 Honest evaluation: held-out splits, leakage checks, Dice / IoU / AJI / panoptic quality, AUC and calibration
- 🚀 End to end: data pipeline → training → evaluation → FastAPI backend → interactive web app

---

## ⭐ Featured projects

### [🧫 Embryo Vision AI](https://github.com/hunzala-sheikh/embryo-vision-ai)
Segmentation and cell counting for embryo microscopy, with a live web app.
- Blastocyst structures (zona pellucida, trophectoderm, inner cell mass, cavity) with Gardner grading
- Time-lapse tracking of embryo development and automatic blastocyst-formation time
- **3D confocal cell segmentation: 93.2% Dice, 80.7% panoptic quality** on held-out data, vs 70% for a standard U-Net
- Dense nucleus separation: **94.4% Dice** on the official test split

`PyTorch` `Attention ResUNet` `Watershed` `FastAPI` `Apple MPS`

### [🦵 KneeWS: Knee MRI from Noisy Reports](https://github.com/hunzala-sheikh/KneeWS)
Multi-label knee MRI diagnosis (12 findings) trained from 4,400+ multilingual radiology reports and only 58 expert labels.
- Local LLM turns reports into labels with quoted evidence; a reliability model weights each label
- DINOv2 2.5D MRI features, scanner-grouped cross-validation, **macro AUC 0.75 with better calibration** than the baseline
- Clinical viewer for DICOM / NIfTI, abstention for uncertain cases, and an expert label-review workflow

`PyTorch` `DINOv2` `Weak supervision` `FastAPI` `Next.js` `PostgreSQL`

### [📉 MLOps Drift-Triggered Retraining](https://github.com/hunzala-sheikh/mlops-drift-composite-trigger)
Detects data and concept drift with a weighted composite score (PSI, KS, performance drop, staleness) and chooses
how much to retrain, keeping production models accurate at lower cost.

`MLOps` `Drift detection` `Python`

---

## 🧰 Tech

**ML / CV:** PyTorch · torchvision · U-Net / ResUNet / HRNet / DeepLabV3 · DINOv2 · scikit-learn · OpenCV · scikit-image
**Medical data:** DICOM · NIfTI · confocal z-stacks · time-lapse microscopy · annotation masks and polygons
**Engineering:** Python · FastAPI · PostgreSQL · Next.js / TypeScript · GitHub Actions

---

💬 Working on a medical or microscopy imaging project and need models trained on your annotated data? Feel free to reach out.
