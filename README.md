# Internship-week-1
Phishing Detection Project Presentation
1. Project Objective
•	Goal: To analyze and understand patterns in website features to distinguish phishing websites from legitimate ones.
•	Importance:
o	Mitigate cybersecurity risks.
o	Protect users from identity theft and financial fraud.

2. Business Problem
•	Phishing Websites:
o	Deceptive sites that mimic legitimate ones to steal sensitive information.
•	Challenges:
o	Constantly evolving tactics by attackers.
o	High potential for false positives in detection.
•	Potential Impact:
o	Enhanced online safety for businesses and individuals.
o	Reduced operational costs related to cybercrime.

3. Dataset Overview
•	Features: 89 features, a mix of numerical and categorical.
•	Target Variable: status (Phishing or Legitimate).
•	Key Features:
o	length_url: Length of the URL.
o	web_traffic: Approximate number of site visitors.
o	domain_age: Age of the domain in days.

4. Data Preprocessing
•	Missing Values:
o	Detected using .isnull().sum().
o	Handled with mean/median imputation.
•	Outliers:
o	Addressed using the Interquartile Range (IQR) method.
•	Encoding:
o	Categorical variables converted to numerical using label encoding.

5. Exploratory Data Analysis (EDA)
Target Variable Distribution
•	Observation:
o	Balanced distribution between phishing and legitimate websites.
•	Visualization:
o	Count plot for status.
Key Insights from Visualizations
•	Histograms:
o	Show patterns in numerical features like length_url.
•	Scatter Plots:
o	Highlight relationships between features such as web_traffic vs. domain_age.
•	Correlation Heatmap:
o	Identified feature interdependencies.
o	Example: Strong correlation between domain_age and legitimacy.

6. Handling Outliers
•	Method:
o	Calculated using IQR.
o	Filtered extreme values beyond 1.5 * IQR range.
•	Result:
o	Cleaner data for reliable analysis.

8. Summary of Findings
•	Key Features for Detection:
o	Short domain age and low web traffic are strong indicators of phishing.
•	Data Quality Issues:
o	Missing values in dns_record and google_index.
o	Addressed outliers in web_traffic and page_rank.

