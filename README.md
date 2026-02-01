## **Predictive Modeling of Employee Attrition at Salifort Motors**

### **Project Overview**

The objective of this project was to address the critical operational and financial challenges posed by high employee turnover at Salifort Motors. By utilizing a dataset of employee survey responses and HR records, I developed three predictive models—Logistic Regression, Decision Tree, and Random Forest—to identify at-risk staff. The analysis successfully uncovered key turnover drivers, such as high workload and inadequate salary, while the **Random Forest model** emerged as the top performer, providing high-accuracy predictions to guide targeted retention strategies.

### **Business Understanding**

The primary stakeholders for this project are the **Salifort Motors HR Department** and **Executive Leadership**. The core business problem is the rising cost of attrition, which includes recruitment expenses, loss of institutional knowledge, and diminished team morale.

In the automotive sector, turnover can be particularly costly; research indicates that replacing a technical or specialized employee can cost between **100% and 150% of their annual salary** (Built In, 2024). Furthermore, high workload and perceived unfairness in compensation are leading indicators of "turnover intention" within manufacturing environments (Journal of Positive School Psychology). This project seeks to mitigate these risks by providing a data-driven early warning system.

### **Data Understanding**

The analysis was conducted using internal survey data collected by the HR department. The dataset captures a comprehensive snapshot of the workforce, including:

* **Operational Metrics:** Monthly hours worked, number of projects, and tenure.
* **Performance & Sentiment:** Last evaluation scores and self-reported satisfaction levels.
* **Organizational Context:** Departmental affiliation and salary level (low, medium, high).
* **Safety & Status:** Work accidents and promotion history within the last five years.

**Data Limitations:** The dataset is a cross-sectional "snapshot," meaning it does not capture changes in employee sentiment over time. Additionally, "satisfaction" is a self-reported metric, which may be subject to response bias.

### **Modeling and Evaluation**

To ensure a robust prediction, I implemented and compared three distinct modeling approaches. The models were evaluated primarily on **F1-Score** and **AUC-ROC** to balance precision and recall, ensuring that we identify as many at-risk employees as possible without excessive false alarms.

| Model | Key Metrics & Strengths |
| --- | --- |
| **Logistic Regression** | Provided a baseline for interpretability and established linear relationships between features like salary and attrition. |
| **Decision Tree** | Captured non-linear patterns, such as the "u-shaped" relationship between workload and turnover (where both very low and very high workloads drive exits). |
| **Random Forest** | **Top Performer.** Delivered the highest predictive accuracy and identified "Number of Projects" and "Average Monthly Hours" as the most influential features. |

### **Conclusion**

The analysis reveals that turnover at Salifort Motors is primarily driven by **extreme workloads** and **stagnant career progression**. To solve these business problems, I recommend the following:

* **Cap Workload:** Implement a threshold for maximum monthly hours and project assignments to prevent burnout.
* **Re-evaluate Compensation:** Conduct a market salary audit for roles in the "high turnover" departments (e.g., Sales) to ensure competitive pay.
* **Improve Internal Mobility:** Establish clear promotion pathways, as a lack of recent promotions was a significant predictor of departure.

**Future Steps:** To expand on this project, I plan to incorporate **Time-Series Analysis** to determine if turnover peaks during specific seasons and integrate **Natural Language Processing (NLP)** on exit interview text data to capture qualitative insights not present in the current survey.
