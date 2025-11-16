# food-delivery-churn
# Customer Churn Prediction (Food Delivery)

Predict customer churn on a simulated Zomato/Blinkit-style dataset using Logistic Regression, with personalized retention offers for high-risk customers.
## 📌 Project overview
Food delivery platforms face churn when users stop ordering. This project:
- Simulates customer data (500 customers)
- Cleans and transforms data using Pandas
- Engineers features like `DaysSinceLastOrder` and `EngagementScore`
- Trains a Logistic Regression model to predict churn
- Assigns risk tiers (Low, Medium, High)
- Suggests retention offers based on churn risk
- Exports results for dashboards or reporting

## ⚙️ Requirements
- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib
- Google Colab (recommended)
  

Install in Colab:
```bash
!pip install pandas numpy scikit-learn matplotlib


## 📂 Dataset
Synthetic dataset with:
- `CustomerID` — unique customer IDs
- `OrderFrequency` — orders per month
- `LastOrder` — date of last order
- `Rating` — satisfaction (1–5)
- `Complaints` — count of complaints


## 🚀 Workflow
1. Data simulation → generate synthetic dataset
2. Data cleaning → handle missing values, convert types
3. Feature engineering → `DaysSinceLastOrder`, `AvgOrderGapDays`, `EngagementScore`
4. Model training → Logistic Regression
5. Evaluation → ROC AUC, classification report
6. Retention offers → rule-based recommendations
7. Export results → CSV outputs


## 📊 Outputs
- `simulated_customers.csv` — synthetic dataset
- `churn_recommendations.csv` — churn risk + retention offers
- ROC curve plot (model evaluation)

Example:
| CustomerID | ChurnRiskProb | RiskTier | RetentionOffer                          |
|------------|---------------|----------|-----------------------------------------|
| 101        | 0.82          | High     | Win-back offer: 30% off + free delivery |
| 245        | 0.55          | Medium   | Reminder: 15% off weekend orders        |
| 390        | 0.12          | Low      | Loyalty rewards: festival early access  |



## 🔮 Future improvements
- Try other models (Random Forest, XGBoost)
- Add features (customer demographics, cuisine preferences)
- Deploy a dashboard (Power BI or Streamlit)
- A/B test retention offers for effectiveness


## 👩‍💻 Author
Created by Tanishka —  focusing on business analytics, Power BI, and data storytelling.


## 📎 How to run
1. Open the notebook in Google Colab.
2. Run cells in order: simulate → clean → engineer features → train → evaluate.
3. Export results as `churn_recommendations.csv`.
4. Upload outputs to GitHub.

