# Titanic Survival Prediction Model

This project is a simple machine learning model that predicts whether a passenger survived the Titanic disaster based on their **Age**, **Sex**, and **Passenger Class (Pclass)**.

The model is built using **Logistic Regression** with data preprocessing and visualization in Python.

---

## 📊 Dataset

- The dataset used is `titanic.csv`, which contains information about passengers aboard the Titanic.
- Features used in this model:
  - `Age` (Numerical)
  - `Sex` (Categorical → Encoded: Male = 0, Female = 1)
  - `Pclass` (1 = 1st class, 2 = 2nd class, 3 = 3rd class)

---

## 🔧 Preprocessing Steps

- Missing values in `Age` were filled with the column's **mean**.
- `Sex` was converted to numerical format using mapping:
  - `'male'` → `0`
  - `'female'` → `1`
- Only three features were selected: `Age`, `Sex`, and `Pclass`.

---

## 🧠 Model

- **Model Type**: Logistic Regression (from `sklearn.linear_model`)
- **Training/Test Split**: 80% training, 20% test
- **Accuracy Achieved**: ~81% on the test set

---

## 🔍 How It Works

After training the model, the notebook accepts live user input:

- **Age**: Integer (e.g., 25)
- **Sex**: `0` for Male, `1` for Female
- **Pclass**: `1`, `2`, or `3`

It then predicts:
- `Survived` (if prediction = 1)
- `Dead` (if prediction = 0)

---

## 🖥️ Example Output

```text
Enter age: 10
Enter sex (Male - 0, Female - 1): 1
Enter pclass (1, 2, 3): 2
Survived
Model accuracy on test set: 0.8100
