# Voter Turnout Prediction Analysis

This project analyzes voter behavior and turnout prediction using a dataset that includes demographic details, historical voting data, and predicted voting probabilities. The objective is to identify patterns that help campaign teams target voters more effectively.

---

## 📊 Problem Summary

Predicting whether a registered voter is likely to vote in the upcoming election using machine learning techniques. By combining historical turnout data and demographic features, the goal is to enable more efficient, data-driven campaign strategies.

---

## 🗃️ Data Overview

The dataset contains the following key features:

- `age`: Age of the voter
- `party`: Political party affiliation
- `vhXXg`: Voting history for past general elections (e.g., `vh12g`, `vh14g`)
- `vote_prob`: Model-generated probability of voting
- `target`: Actual turnout label (1 = voted, 0 = did not vote)

---

## 📈 Model Performance

A classification model was trained and evaluated. The classification report shows perfect precision, recall, and F1-score:

| Metric     | Score  |
|------------|--------|
| Precision  | 1.00   |
| Recall     | 1.00   |
| F1-Score   | 1.00   |
| Accuracy   | 1.00   |

> Total samples: 1,703

---

## 🔍 Key Insights

- **Age**: Older voters are generally more likely to vote.
- **Vote History**: Previous turnout (`vh12g`, `vh14g`, etc.) is a strong predictor of future voting behavior.
- **Party Affiliation**: Certain parties have higher turnout probabilities.
- **Vote Probability Distribution**: Most predicted probabilities are concentrated near 0 or 1, indicating high model confidence.

---

## 📌 Visualizations

- **Histogram**: Distribution of predicted vote probabilities
- **Pie Chart**: Actual turnout distribution (voted vs did not vote)
- **Feature Importance** (optional): Use SHAP or permutation importance to analyze contributing factors

---

## 🚀 Next Steps

1. **Field Targeting**: Use predicted probabilities to segment voters into likely, swing, and unlikely groups for tailored outreach.
2. **Resource Allocation**: Prioritize high-impact voters in competitive districts.
3. **Model Updates**: Retrain the model with real-time data for better performance ahead of future elections.
4. **Dashboard Integration**: Deploy insights into a campaign dashboard for field teams.

---

## 📁 Files

- `voterTurnoutPredictions.csv`: Dataset
- `model.ipynb`: Code for training, evaluation, and visualization
- `README.md`: Project documentation

---

## ✅ Requirements

- Python 3.7+
- pandas
- matplotlib
- seaborn
- scikit-learn

Install dependencies with:

```bash
pip install -r requirements.txt
