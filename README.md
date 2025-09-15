# 🌾 Crop & Fertilizer Recommendation System

A Machine Learning-based system to recommend the best crop to grow and the most suitable fertilizer to use, based on soil and environmental parameters such as **N, P, K values, temperature, humidity, pH, and rainfall**.  
This project uses data-driven insights to support better farming decisions and is developed as part of the **EDUNET program (Week 1–3)**.

---

## 🛠 Tech Stack
- **Python 3.x**
- **Jupyter Notebook**
- **Libraries:** Pandas, NumPy, Scikit-learn
- **Model Saving:** Pickle (`.sav` files)

---

## 📂 Repository Structure

```
├── Data-processed/
│   ├── crop_recommendation.csv          # Processed dataset for crop recommendation
│   ├── fertilizer.csv                   # Processed dataset for fertilizer recommendation
│
├── Data-raw/
│   ├── Fertilizer.csv                   # Raw fertilizer dataset
│   ├── FertilizerData.csv               # Alternate raw fertilizer data
│   ├── MergeFileCrop.csv                # Raw merged crop dataset
│   ├── cpdata.csv                       # Raw crop dataset
│   ├── raw_districtwise_yield_data.csv  # District-level raw yield dataset
│
├── models/
│   ├── crop_model.sav                   # Trained crop recommendation model
│   ├── crop_scaler.sav                  # Scaler used for crop model
│   ├── fertilizer_model.sav             # Trained fertilizer recommendation model
│   ├── fertilizer_scaler.sav            # Scaler used for fertilizer model
│
├── notebooks/
│   ├── Crop_Recommendation_Model.ipynb        # Crop recommendation model building
│   ├── Crop_data_preparation.ipynb            # Data preprocessing and cleaning
│   ├── Final_recommendationdata_creation.ipynb # Dataset preparation for recommendations
│
├── .gitignore
├── README.md
├── requirements.txt
```

## 🚀 Features

- **Crop Recommendation**: Suggests the most suitable crop based on soil and weather conditions.
- **Fertilizer Recommendation**: Provides the right fertilizer suggestions based on soil nutrient balance.
- **Data Pipelines**: Prepares raw agricultural data into structured datasets.
- **Trained Models**: Saved models (`.sav`) available for direct reuse.
- **Jupyter Workflows**: Notebooks covering data cleaning, model training, and dataset preparation.

---

## 📈 Project Progress (Week-wise Improvements)

### 🔹 Week 1
- Selected relevant agricultural datasets.
- Understood dataset features (N, P, K, temperature, humidity, pH, rainfall, etc.).
- Performed **basic preprocessing and cleaning** (handling null values, formatting).

### 🔹 Week 2
- Enhanced preprocessing: scaling, encoding, and handling inconsistencies.
- Cleaned and merged multiple raw datasets from `Data-raw/`.
- Created structured datasets in `Data-processed/` for ML training.

### 🔹 Week 3
- Built **Crop Recommendation Model** and **Fertilizer Recommendation Model**.
- Saved trained models and scalers (`.sav` files in `models/`).
- Finalized recommendation dataset using `Final_recommendationdata_creation.ipynb`.
- Completed end-to-end pipeline from raw data → processed data → trained models.

---

## 💡 How to Use

1. **Clone the repository**
    ```bash
    git clone <your-repo-link>
    cd <your-repo-folder>
    ```

2. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3. **Run Notebooks**
    - Preprocess data: `notebooks/Crop_data_preparation.ipynb`
    - Train crop model: `notebooks/Crop_Recommendation_Model.ipynb`
    - Generate final dataset: `notebooks/Final_recommendationdata_creation.ipynb`

4. **Use Trained Models**
    - Load models from the `models/` folder (`.sav` files) for direct prediction without retraining.

---

## ✅ Outcome

- Processed datasets ready for reuse (`Data-processed/`).
- Trained ML models and scalers saved in `models/`.
- Complete ML pipeline documented in Jupyter notebooks.
- Crop & Fertilizer Recommendation System prototype completed.

---

## 🔮 Future Enhancements

- Develop a **user interface (web/desktop app)** for farmers.
- Integrate **real-time weather APIs** for dynamic recommendations.
- Expand dataset with more crops, regions, and fertilizer types.
- Deploy trained models as an **API or Streamlit app** for broader accessibility.
