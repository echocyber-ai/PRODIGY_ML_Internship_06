# House Price Prediction: Regression Analysis Comparison

## 📌 Project Overview
This project involves developing a machine learning pipeline to predict real estate prices based on structural and geographical features. The core objective was to implement a robust regression model and evaluate its performance against a baseline to ensure the highest possible predictive accuracy.

## 📊 Dataset
The project utilizes the **King County House Sales Dataset** (Seattle, USA). 
* **Target Variable:** `price`
* **Features:** `bedrooms`, `bathrooms`, `sqft_living` (Size), `lat` (Latitude), and `long` (Longitude).

## 🔬 Methodology
The data underwent a rigorous preprocessing phase:
1.  **Feature Selection:** Narrowed down variables to the most impactful structural and locational data points.
2.  **Standardization:** Applied `StandardScaler` to normalize features, ensuring that the model is not biased toward larger numerical scales (like square footage).
3.  **Comparative Modeling:** Two distinct algorithms were trained and tested:
    * **Linear Regression:** Used as a baseline to test linear relationships.
    * **Gradient Boosting Regressor:** Used to capture complex, non-linear dependencies.

## 📈 Model Comparison & Selection
After evaluating both models on unseen test data, the following results were observed:

| Model | MAE (Mean Absolute Error) | RMSE (Root Mean Squared Error) |
| :--- | :--- | :--- |
| **Linear Regression** | High | High |
| **Gradient Boosting** | **Significantly Lower** | **Significantly Lower** |

### Decision Logic:
While Linear Regression provided a quick baseline, it failed to account for the "Location" factor accurately. **Gradient Boosting** was chosen as the final model because its ensemble nature allowed it to learn specific high-value geographical clusters, resulting in a much tighter fit between actual and predicted prices.



## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn
* **Visualization:** Matplotlib, Seaborn

## 💡 Key Results
The final Gradient Boosting model shows a strong linear trend in the "Actual vs. Predicted" scatter plot, successfully minimizing error across the majority of the housing market spectrum.

## 👩‍💻 Author
**Eshaal Hammad**
* **Email:** eshaalhammad234@gmail.com
