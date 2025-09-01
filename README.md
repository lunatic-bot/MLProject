# Score Predictor App

This is a small end-to-end **Score Prediction** application that predicts scores based on user input. The project is structured in a **modular** way using pipelines and reusable components to maintain clean and readable code.

## Project Highlights

- Modular project architecture using custom **pipelines** and **components**
- Machine Learning models implemented and compared
- Frontend built with **HTML** and **CSS**
- Backend powered by **Flask**
- Deployed on **Azure App Service** using **GitHub Actions CI/CD**

---

## ML Models Used

The following regression models were trained and evaluated:

```python
models = {
    "Random Forest": RandomForestRegressor(),
    "Decision Tree": DecisionTreeRegressor(),
    "Gradient Boosting": GradientBoostingRegressor(),
    "Linear Regression": LinearRegression(),
    "XGBRegressor": XGBRegressor(),
    "CatBoosting Regressor": CatBoostRegressor(verbose=False),
    "AdaBoost Regressor": AdaBoostRegressor(),
}
```

````

Each model was tested and evaluated using performance metrics like R² score to find the best fit for the dataset.

---

## Tech Stack

| Layer      | Tools Used                         |
| ---------- | ---------------------------------- |
| Frontend   | HTML, CSS                          |
| Backend    | Flask                              |
| ML Models  | Scikit-learn, XGBoost, CatBoost    |
| Deployment | Azure App Service + GitHub Actions |

---

## Deployment

The app is deployed on Azure Web App with an automated **GitHub Actions pipeline** for continuous integration and delivery.

You can access it via:

```
http://score-prediction-hqh6esdrdwazchbc.canadacentral-01.azurewebsites.net
```

---

## How to Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/lunatic-bot/MLProject.git
   cd project
   ```

2. Create a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the Flask app:

   ```bash
   python application.py
   ```

5. Open in browser:

   ```
   http://localhost:5000/
   ```

---

## Feedback

If you find any issues or want to suggest improvements, feel free to raise an issue or submit a PR.

```
````
