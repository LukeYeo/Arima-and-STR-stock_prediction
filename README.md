# 📈 Stock Price Prediction Using Neural Networks (Amazon Stock)

This project explores the application of **neural networks** to forecast the future stock price of **Amazon (AMZN)**. It involves preparing time-series financial data, training a neural network model, and evaluating its predictive accuracy using historical data.

This work was completed as part of an academic assignment for **DATA2001** at the University of Queensland.

---

## 👨‍💻 Author

**Yeo Chee En Luke**  
Student Number: 46746267  
Assignment: DATA2001 - Assignment 2 (Insight)

---

## 🧰 Tools & Technologies Used

| Tool / Library     | Purpose                                   |
|--------------------|-------------------------------------------|
| Python             | Programming language                      |
| Pandas             | Data loading and preprocessing            |
| NumPy              | Numerical operations                      |
| Matplotlib         | Data visualization                        |
| Keras / TensorFlow | Neural network modeling and training      |
| Scikit-learn       | Preprocessing and evaluation              |

---

## 📁 Dataset

- **Source:** `amzn.us.csv` — historical Amazon stock data.
- The dataset includes features like `Open`, `Close`, `High`, `Low`, and `Volume`.

---

## 🔄 Project Workflow

### 1. 📊 Data Preparation

- Imported CSV with `Date` as index.
- Visualized trends and missing data.
- Scaled features using `MinMaxScaler`.

### 2. 🧠 Neural Network Modeling

- Built a feedforward neural network using **Keras**.
- Input: multiple stock features from prior days.
- Output: predicted `Close` price.
- Model architecture includes:
  - Input layer (dense)
  - Hidden layers (ReLU activations)
  - Output layer (linear)

```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense

model = Sequential()
model.add(Dense(128, activation='relu', input_shape=(n_features,)))
model.add(Dense(64, activation='relu'))
model.add(Dense(1))  # Output: predicted close price
model.compile(optimizer='adam', loss='mean_squared_error')
```

### 3. 🧪 Training & Evaluation

- Split dataset into training and test sets.
- Trained for multiple epochs using MSE loss.
- Evaluated with:
  - **RMSE**
  - **Visual comparison of predicted vs actual prices**

### 4. 📈 Visualization

- Line plots comparing **predicted** and **actual** stock prices.
- Highlighted how well the model captured the stock’s upward or downward movement.

---

## ✅ Key Results

- The model was able to **approximate short-term movements** of Amazon’s stock.
- Achieved reasonable performance with limited features (no macroeconomic indicators).
- Demonstrated how machine learning can be applied to financial forecasting.

---

## 📚 Skills Demonstrated

- Time-series preprocessing
- Neural network design with Keras
- Training/evaluation of regression models
- Visualization for insight communication
- Understanding limitations of stock prediction

---

## ⚠️ Disclaimer

This project was done for **learning and academic purposes** only. It should not be used for investment or trading decisions.

---

## 🧑‍🏫 Acknowledgement

This project was submitted as part of **DATA2001** at the University of Queensland. The dataset was provided as part of the assignment instructions.

---
