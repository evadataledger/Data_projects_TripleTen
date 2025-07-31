# Project 14: Computer Vision – Good Seed Age Verification

## Objective
Build and evaluate a computer vision model to determine whether a customer is of legal age to purchase alcohol using checkout camera images. This supports **Good Seed** supermarkets in compliance with alcohol sales regulations.

---

## Dataset
- 7.6k photos labeled with real age
- `labels.csv` — contains image file names and corresponding real ages
- Image Directory: `/datasets/faces/final_files/`

> ⚠Due to GitHub size limits, image files are **not** included. Reference paths and sample visualizations are documented in the notebook.

### Dataset Source
The dataset was obtained from:  
[ChaLearn Looking at People](https://gesture.chalearn.org/)  
(*Alternate URL [chalearnlap.cvc.uab.cat](https://chalearnlap.cvc.uab.cat/) appears to be inactive.*)

---

## Project Tasks
- **EDA (Exploratory Data Analysis)**:
  - Visualized age distribution
  - Displayed sample images for various ages
  - Analyzed potential impact of age distribution on model training

- **Model Development**:
  - CNN with **ResNet50** backbone (pretrained on ImageNet)
  - ReLU activation for regression (age prediction)
  - Optimized with `Adam`, evaluated with `MAE` (Mean Absolute Error)

- **Training Summary**:
  - Trained for 20 epochs on GPU
  - Final MAE: **~7.65** years on validation data
  - Overfitting observed in later epochs → potential regularization opportunity

---

## Evaluation

| Epoch | MAE (Validation) | Loss (Validation) |
|-------|------------------|-------------------|
| 6     | 7.03             | 85.10             |
| 8     | 6.72             | 80.00             |
| 20    | **7.65**         | 93.41             |

---

## Key Insights
- Model learns effectively in early epochs
- Data imbalance across age groups may skew performance
- Further improvement possible with:
  - Data Augmentation
  - Class Rebalancing
  - Early Stopping & Dropout Regularization

---

## Tools Used
- Python
- TensorFlow/Keras
- ResNet50 (Transfer Learning)
- Matplotlib & Seaborn for visualization

---

## Note
Model training was completed externally due to GPU limitations.  
Large image datasets are not hosted in this repository — paths and samples are referenced only.

---

## Folder Structure

```bash
project_14_computer_vision/
├── notebooks/
│ └── Project_14_Computer_Vision_GoodSeed.ipynb
├── README.md
├── requirements.txt

