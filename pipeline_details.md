# Pipeline Configuration & Model Summaries

## 1. Sleep Time Ratio (%) `[Sleep_Ratio]`
* **Data Split:** Train days: 99 | Test days: 25 (Sequences: 96 Train, 22 Test)

### Model Architectures & Best Parameters
* **Random Forest:** `{'max_depth': 10, 'max_features': 'sqrt', 'min_samples_split': 5, 'n_estimators': 200}`
* **LSTM Configuration:** * Units: 50 | Dropout: 0.2 | Dense Units: 25 | Window Size: 3 days
  * Epochs: 50 | Batch Size: 8 | Optimizer: Adam | Loss: MSE

---

## 2. Sleep Stages - Deep Sleep (min) `[Deep_Sleep]`
* **Data Split:** Train days: 99 | Test days: 25 (Sequences: 96 Train, 22 Test)

### Model Architectures & Best Parameters
* **Random Forest:** `{'max_depth': None, 'max_features': 'sqrt', 'min_samples_split': 2, 'n_estimators': 200}`
* **LSTM Configuration:** * Units: 50 | Dropout: 0.2 | Dense Units: 25 | Window Size: 3 days
  * Epochs: 50 | Batch Size: 8 | Optimizer: Adam | Loss: MSE

---

## 3. Sleep Stages - Awake (min) `[WASO]`
* **Data Split:** Train days: 99 | Test days: 25 (Sequences: 96 Train, 22 Test)

### Model Architectures & Best Parameters
* **Random Forest:** `{'max_depth': 10, 'max_features': 'sqrt', 'min_samples_split': 5, 'n_estimators': 100}`
* **LSTM Configuration:** * Units: 50 | Dropout: 0.2 | Dense Units: 25 | Window Size: 3 days
  * Epochs: 50 | Batch Size: 8 | Optimizer: Adam | Loss: MSE