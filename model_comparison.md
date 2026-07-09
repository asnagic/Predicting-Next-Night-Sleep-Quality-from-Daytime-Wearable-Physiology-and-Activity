# Clinical Performance Comparison

## Overall Performance Metrics

| Target | Model | MAE | RMSE | R² | MAPE (%) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Sleep Time Ratio (%)** | Random Forest | 3.056555 | 3.757306 | 0.290243 | 3.602253 |
| | LSTM | 4.198643 | 5.107250 | -0.176329 | 4.856238 |
| **Sleep Stages - Deep Sleep (min)** | Random Forest | 38.275400 | 54.716102 | -0.068368 | 47.862114 |
| | LSTM | 40.059025 | 55.205918 | -0.008215 | 54.136705 |
| **Sleep Stages - Awake (min)** | Random Forest | 27.447387 | 34.360386 | -0.256586 | 84.682523 |
| | LSTM | 28.719600 | 36.758423 | -0.312501 | 93.417517 |

---

## LSTM vs. Random Forest Comparative Analysis

| Target | Label | LSTM MAE | LSTM R² | RF MAE | RF R² | MAE Difference (RF - LSTM) | R² Difference (RF - LSTM) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Sleep Time Ratio (%)** | Sleep_Ratio | 4.1986 | -0.1763 | 3.0566 | 0.2902 | -1.1421 | 0.4666 |
| **Sleep Stages - Deep Sleep (min)** | Deep_Sleep | 40.0590 | -0.0082 | 38.2754 | -0.0684 | -1.7836 | -0.0602 |
| **Sleep Stages - Awake (min)** | WASO | 28.7196 | -0.3125 | 27.4474 | -0.2566 | -1.2722 | 0.0559 |

> **Note:** Positive differences indicate Random Forest outperforms LSTM.