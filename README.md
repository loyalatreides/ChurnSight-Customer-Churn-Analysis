# 🧠 ChurnSight — Customer Churn Prediction & Retention Analysis  

**Author:** Kamran Habib  
**Tools:** Azure Databricks (PySpark + MLlib) | Power BI | MLflow  
**Focus:** Data Engineering · Machine Learning · Business Intelligence  

---

## 📌 Business Objective  
Telecom providers face significant revenue loss from customer churn.  
**ChurnSight** predicts which customers are likely to churn, explains *why*, and prioritizes *whom to retain* based on RFM value and churn probability.

---

## ⚙️ Technical Workflow  

| Stage | Platform | Key Tasks |
|-------|-----------|-----------|
| **Data Engineering** | Azure Databricks | Loaded and cleaned IBM Telco Churn dataset, handled missing `TotalCharges`, encoded categoricals, built feature vectors. |
| **Modeling** | PySpark MLlib | Compared 4 models – LR, DT, RF, GBT → **Logistic Regression** chosen (AUC 0.858 · F1 0.809). |
| **Feature Enrichment** | PySpark | Calculated RFM (Recency–Frequency–Monetary) and Retention Priority = `RFM × Churn Probability`. |
| **Visualization** | Power BI | Created multi-page dashboard (Data Overview · Churn Analysis · Retention & RFM · Executive Summary). |

---

## 📊 Power BI Highlights  

- **Data Overview:** KPIs (Total Customers 2004, Churn Rate 26.6 %, Avg RFM 8.9)  
- **Churn Analysis:** Highest risk → Month-to-Month contracts, Fiber Internet users.  
- **Retention & RFM:** 107 high-value customers at high risk; scatter of RetentionPriority vs Churn Probability.  
- **Executive Summary:** Leadership dashboard summarizing KPIs & drivers.

---

## 💡 Key Insights  

| Question | Finding |
|-----------|----------|
| Who is likely to churn? | 26 % of customers predicted to churn — mostly Month-to-Month & Fiber users. |
| Why are they churning? | High monthly charges, short contracts, electronic payment methods. |
| Who is worth retaining? | 107 customers with RFM > 8 and Churn Probability > 0.6. |

---

## 📈 Business Impact  

- Potential **10–15 % churn reduction** through targeted retention.  
- **\$100 K+ annual revenue** saved from high-value customers.  
- Enabled data-driven, proactive retention strategy.

---

## 🧰 Skills Demonstrated  
- **Data Engineering:** PySpark, Databricks FileStore, Feature Pipelines  
- **Machine Learning:** Model tuning (AUC, F1), MLflow tracking  
- **Visualization:** DAX measures, calculated columns, multi-page Power BI reports  
- **Business Analytics:** RFM scoring, customer segmentation, churn risk modelling  

---
## 🔗 Links

- 📄 [ChurnSight Report (PDF)](ChurnSight%20Report.pdf)
- 📊 [Power BI Dashboards (PDF)](ChurnSight%20PBI.pdf)
- 🧠 [Databricks Notebook (HTML)](Phase2_Churn_ML2.html)
- 🧾 [Final Scored Dataset (CSV)](final_scored.csv)

---

## 📅 Next Steps  
- Automate model scoring via Azure ML pipeline.  
- Integrate real-time CRM data feeds.  
- Publish Power BI Service dashboard for executives.  

---

⭐ **If you like this project, star the repo!**  
