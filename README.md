# User Churn Prediction
<p align="justify"> Waze’s complimentary navigation application enhances global driving experiences by simplifying route planning. The platform benefits from a collaborative network of map editors, beta testers, translators, partners, and users, all contributing to safer and more efficient journeys. Waze collaborates with municipalities, transportation authorities, media outlets, businesses, and emergency responders to optimize travel for a broader audience. </p>

<p align="justify"> This initiative is part of Waze’s broader strategy to drive growth. High retention rates typically reflect user satisfaction and consistent app usage. By developing a churn prediction model, Waze aims to mitigate user attrition, bolster retention, and expand its business. An accurate model will also pinpoint key factors influencing churn. </p>

### **Overview**
<p align="justify"> The aim of this project was to develop a machine learning model to predict user churn, which measures the number of users who have uninstalled or stopped using the Waze app. The project specifically targets monthly user churn. Two tree-based models, the random forest and XGBoost, were created and evaluated. The objective of this model is to identify factors that drive user churn and to predict whether a Waze user will be retained or churn. The final selected model, XGBoost, achieved an accuracy of 71% and a recall of 51%. Key factors influencing user retention versus churn, according to the model, include km_per_hour, n_days_after_onboarding, percent_sessions_in_last_month, and total_sessions_per_day. </p>

### **Business Understanding**
<p align="justify"> This initiative will enable leadership to make well-informed business decisions aimed at reducing user churn, enhancing user retention, and expanding Waze’s business. By identifying users at high risk of leaving, Waze can take proactive steps to keep them engaged. For instance, recognizing a high-risk user segment allows Waze to offer special incentives to retain these users. </p>

### **Data Understanding**
<p align="justify"> The dataset comprised 14,999 entries and 13 features. These features encompassed data such as the frequency of app openings by a user within the month, the type of device used to start a session, the number of days since the user registered for the app, the total kilometers driven during the month, and the number of days the app was accessed by the user within the month. The pie chart below illustrates the distribution of users by device type. </p>

![image](https://github.com/user-attachments/assets/3f261003-b498-4ecb-9a30-9a592077e75a)

There are nearly twice as many iPhone users as Android users represented in this data.

A histogram that, for each day, has a bar representing the counts of driving_days and activity_days.

![image](https://github.com/user-attachments/assets/4a13d87b-5f4a-4220-8973-a0c527f8003e)

A histogram that has four bars—one for each device-label combination—to show how many iPhone users were retained/churned and how many Android users were retained/churned.

![image](https://github.com/user-attachments/assets/f47e314c-602e-485e-b2d9-5abe6fe8d871)

Another histogram represents the churn rate for each number of driving days.

![image](https://github.com/user-attachments/assets/f7418a79-d81f-4117-9b49-f3c68f657623)

### **Modeling and Evaluation**
<p align="justify"> An XGBoost model with 400 decision trees was employed to identify the key features influencing user churn. The plot below highlights the top four most significant factors in predicting user churn. The model achieved an overall accuracy of 67% and a recall of 59%. </p>

### **Conclusion**
<p align="justify"> This model can assist Waze leadership in making informed business decisions to reduce user churn. By identifying the key factors driving churn, the model enables Waze to implement proactive strategies to retain users who are at risk of discontinuing their use of the app. </p>
