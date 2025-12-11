# ☀️ Solar Energy Prediction with Machine Learning (Upgraded)

Welcome to the **Solar Energy Prediction** repository! This project utilizes refined machine learning techniques to predict solar energy output based on historical data. The analysis is performed using Python, with a focus on stability, accuracy, and efficiency.

---

## 📖 Introduction and Project Goal

Solar energy prediction is crucial for optimizing energy production and managing resources efficiently. This project aims to accurately forecast continuous solar energy output by analyzing historical weather and solar data using advanced machine learning models.

I focused on **fixing statistical inconsistencies** and **optimizing model training** to achieve the highest performance reliably on standard hardware.

---

## ✨ Key Upgrades and Features

* **Robust Data Integrity:** I corrected the initial flaw of multiplying the target variable by 100, which now allows for accurate and meaningful measurement of $\text{RMSE}$.
* **Statistically Valid Feature Selection:** I replaced the incorrect $\chi^2$ test with the appropriate **ANOVA F-value ($\text{f\_regression}$) test** for accurate feature importance ranking. 
* **Optimized XGBoost Regressor:** I implemented a lightweight configuration by reducing complexity (e.g., $\text{max\_depth}=5$, $\text{n\_jobs}=1$) and utilizing **Early Stopping** for faster, memory-safe training and improved generalization.
* **High Performance:** The optimized model achieved an excellent $\text{R}^2$ of $0.93$.

---

## 📈 Final Results and Model Performance

The **XGBoost Regressor** proved to be the most stable, reliable, and high-performing model for this solar dataset.

| Model | Primary Advantage | **Achieved Performance** |
| :--- | :--- | :--- |
| **XGBoost Regressor** | Highest speed, stability, and predictive power. | **$R^2$: 0.93** (Explaining 93% of variability) **$RMSE$: 83.55** |

> **Note on Deep Learning:** *The complex Multilayer Perceptron (MLP) model from the original project was found to be numerically unstable (resulting in `loss: nan` errors) on this dataset and was excluded from the final deliverable, prioritizing the robust XGBoost solution.*

---

## 🛠️ Installation Instructions

Clone the repository:

git clone [https://github.com/a-a-qasim/Solar-Energy-Prediction-with-Machine-Learning.git](https://github.com/a-a-qasim/Solar-Energy-Prediction-with-Machine-Learning.git)
cd Solar-Energy-Prediction-with-Machine-Learning

---

Contributions to this project are highly welcome! If you have ideas for adding new features or further optimizing model hyperparameters, please feel free to fork the repository and submit a pull request.

📬 Contact
For any questions or feedback, feel free to reach out via GitHub Issues or contact me directly.

I harnessed the power of the sun with data-driven insights! ☀️