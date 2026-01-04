# Spatial–Temporal LULC Analysis of Diamer District using Machine Learning

This repository contains the implementation and analysis for the project **“Spatial–Temporal Analysis of Vegetation Cover Change (LULC) in Diamer using Geospatial Techniques and Supervised Classification.”** The study applies supervised machine learning models to classify land use and land cover types in Diamer District, Gilgit-Baltistan, using multispectral satellite imagery.

The goal of this project is to accurately map and monitor changes in vegetation, barren land, water bodies, and built-up/agricultural areas in a complex mountainous environment, and to evaluate the performance of different machine learning classifiers for remote sensing applications.

---

## 📍 Study Area
Diamer District is located in Gilgit-Baltistan, Pakistan. It is a mountainous region characterized by:
- High topographic variation
- Strong spectral heterogeneity
- Seasonal snow cover
- Fragile ecosystems sensitive to climate and land-use change

These characteristics make traditional classification methods less reliable, motivating the use of machine learning techniques.

---

## 🛰️ Data
- **Satellite Source:** Landsat-8 OLI Level-2 Surface Reflectance  
- **Features Used:**
  - Visible, Near Infrared (NIR), and Shortwave Infrared (SWIR) bands
  - Normalized Difference Vegetation Index (NDVI)
- **Classes:**
  - Barren Land
  - Vegetation / Shrubs
  - Water Bodies
  - Agriculture / Built-up

Training samples were generated using visual interpretation and ancillary data. A stratified 70/30 train-test split was applied.

---

## ⚙️ Methodology
The workflow includes:

1. Data acquisition and preprocessing (atmospheric correction, cloud masking, alignment)
2. Feature extraction (spectral bands + NDVI)
3. Data preparation and standardization
4. Model training and testing
5. Accuracy assessment using confusion matrices and statistical metrics
6. Comparative performance evaluation
7. Temporal change analysis and interpretation

---

## 🤖 Machine Learning Models
The following supervised classifiers were implemented and evaluated:

- **Support Vector Machine (SVM)**
- **Random Forest (RF)**
- **Extreme Gradient Boosting (XGBoost)**

Each model was assessed using:
- Overall Accuracy
- Precision, Recall, and F1-Score
- Kappa Coefficient
- Matthews Correlation Coefficient (MCC)

---

## 📊 Results
All models achieved very high performance (>99.7% accuracy). However:

- **XGBoost** achieved the highest overall accuracy and robustness.
- **Random Forest** showed very stable and reliable generalization.
- **SVM** performed well but slightly lower than ensemble models in complex class overlaps.

This confirms that ensemble learning methods are better suited for complex mountainous terrain.

---

## 🌱 Applications
- Environmental monitoring
- Vegetation change detection
- Land-use planning
- Climate change impact assessment
- Sustainable development and resource management

---

## 🧰 Technologies Used
- Python
- NumPy, Pandas
- Scikit-learn
- XGBoost
- Matplotlib
- GIS & Remote Sensing concepts

---

## 📚 References
This work is based on established literature including:
- Breiman (2001) – Random Forest
- Chen & Guestrin (2016) – XGBoost
- Mountrakis et al. (2011) – SVM in remote sensing
- USGS Landsat documentation

(Full references are provided in the accompanying report.)

---

## 👤 Author
**Mehtab Ali**  
Silicon Global Tech, Gilgit-Baltistan  
Course: Data Sciences and Machine Learning  
Supervisor: Hafiz-ud-Din

---

## 📄 License
This project is intended for academic and research use.
