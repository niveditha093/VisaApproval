# VisaApproval
**Context:**

In the United States, businesses face a persistent challenge in identifying and attracting the right talent to stay competitive. The Immigration and Nationality Act (INA) allows foreign workers to contribute to the U.S. workforce temporarily or permanently, with a focus on protecting local workers. The Office of Foreign Labor Certification (OFLC) administers immigration programs, processing applications from employers seeking foreign workers.

**Business Objective:**

In Fiscal Year 2016, the OFLC managed a substantial increase in employer applications, reaching 775,979 for 1,699,957 positions. The escalating number of applicants underscores the need for an efficient solution to sift through candidates and enhance the visa approval process. EasyVisa, engaged by OFLC, aims to leverage machine learning to streamline visa approvals, providing insights to identify candidates with higher visa success probabilities based on influential factors. The data scientist's role is to analyze the dataset and develop a classification model that not only expedites the visa approval process but also recommends suitable profiles for certification or denial based on key drivers influencing case status.

**Business Analysis and Recommendations:**

**1. Visa Approval Facilitation:**
The EasyVisa ML model, particularly the tuned Random Forest classifier, exhibits robust performance with an F1 score of 82% on the test data. The model is well-calibrated, providing accurate predictions for both visa certifications and denials without overfitting. This efficiency can significantly enhance the visa approval process, streamlining the identification of candidates with higher chances of success.

**2. Key Drivers Influencing Case Status:**
   - **Educational Background:** The level of education is a crucial determinant. Applicants with a Doctorate degree have the highest chances of visa certification (over 86%), while those with only a high school certification face a lower likelihood (less than 35%). 
   - **Wage Unit:** The unit of wage plays a vital role, with hourly wages having a lower certification rate (35%) compared to non-hourly pay (70%). 
   - **Job Experience:** Applicants with prior job experience significantly contribute to a higher certification rate (75%) compared to those without (56%).
   - **Region of Employment:** The Midwest region is associated with a higher likelihood of certification (75%), outperforming other regions.
   - **Continent:** Applicants from Europe demonstrate the highest certification rate (80%), followed by Africa, Asia, Oceania, North America, and South America.

**3. Model Interpretability and Efficiency:**
   - **Feature Importance:** The Random Forest model identifies key features influencing predictions. Notably, education, prevailing wage, job experience, and region of employment are among the most influential factors.
   - **Model Efficiency:** The model's efficiency is evident in its ability to generalize well to unseen data, avoiding overfitting. This ensures reliable predictions and facilitates quicker decision-making in the visa approval process.

**4. Data Completeness and Quality:**
   - **Completeness:** The dataset shows no missing values, contributing to the model's reliability.
   - **Numeric Variables:** The analysis of numeric variables, including prevailing wage and employer attributes, reveals insights into prevailing wage distribution and potential outliers.

**5. Operational Considerations:**
   - **Resource Allocation:** Focus on candidates with higher education, relevant job experience, and willingness to work under non-hourly pay terms, as these attributes positively influence visa certification.
   - **Enhanced Review Process:** Given the model's higher recall for certified cases, consider revisiting denied cases, particularly in situations of prevailing human resource shortages.

**6. Continuous Improvement:**
   - **Model Iteration:** Regularly update and refine the model based on new data to adapt to evolving trends and ensure sustained accuracy.
   - **Feedback Mechanism:** Establish a feedback loop with OFLC to incorporate domain-specific insights and continuously enhance model performance.

EasyVisa's machine learning solution not only expedites the visa approval process but also provides actionable insights for strategic decision-making in talent acquisition and compliance with immigration regulations.
