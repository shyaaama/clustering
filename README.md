# Customer Segmentation for Marketing Strategy

## Project Overview
This project aims to analyze customer data from a banking institution to identify distinct customer segments. By utilizing clustering techniques, the project develops personalized marketing strategies to enhance customer satisfaction and increase subscriptions to term deposits.

## Table of Contents
- [Dataset Description](#dataset-description)
- [Technologies Used](#technologies-used)
- [Data Preprocessing](#data-preprocessing)
- [Clustering Techniques](#clustering-techniques)
- [Segment Analysis](#segment-analysis)
- [Marketing Strategies](#marketing-strategies)
- [Conclusion](#conclusion)


## Dataset Description
The dataset consists of **31,647** records with **18 features**, including:
- `customer_age`: Age of the customer.
- `job_type`: Type of job held by the customer.
- `marital`: Marital status (e.g., single, married).
- `education`: Level of education.
- `balance`: Customer’s bank balance.
- `term_deposit_subscribed`: Target variable indicating if the customer subscribed to a term deposit (1 for yes, 0 for no).
-`housing_loan`: Indicates whether the customer has a housing loan (yes/no). Existing loans may influence a customer’s decision to subscribe to additional financial products.
-`personal_loan`: Indicates whether the customer has a personal loan (yes/no). Similar to housing loans, personal loans might affect a customer’s financial decisions.
-`communication_type`: The type of communication used in the campaign (e.g., cellular, unknown). This could indicate the method through which the campaign was conducted.
-`day_of_month`: The specific day of the month when the last contact with the customer was made. Timing of contact might play a role in the campaign's effectiveness.
-`month`: The month in which the last contact was made. Seasonal trends might influence customer behavior.
-`last_contact_duration`: The duration (in seconds) of the last contact with the customer. Longer conversations might indicate higher interest.
-`num_contacts_in_campaign`: The number of contacts made during the current campaign. More contacts could imply persistence or customer interest.
-`days_since_prev_campaign_contact`: The number of days since the last contact in a previous campaign. A shorter gap might influence the likelihood of a positive response.
-`num_contacts_prev_campaign`: The number of contacts made in previous campaigns. This might indicate previous efforts to convert the customer.
-`prev_campaign_outcome`: The outcome of the previous campaign (e.g., success, failure). Past behavior is often a predictor of future actions.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab (for notebook execution)

## Data Preprocessing
- Handled missing values using median or mode imputation.
- Removed outliers based on the Interquartile Range (IQR) method.
- Encoded categorical variables using OneHotEncoder.
- Scaled numerical features for better clustering performance.
- Feature selection
- Hopkin statistics
- Use PCA for dimensionality reduction.

## Clustering Techniques
- Applied **KMeans**,**DBSCAN**,**heirarchical clustering(agglomerative)** and selected **kmeans** as best and clustered to segment customers based on various features.
- Fine tuned it and selected 4 as the best number of cluster using ELBOW METHOD and visualized using KElbowVisualizer
- Evaluated cluster performance using Silhouette and Davies-Bouldin scores.
- Visualized clusters. 

## Segment Analysis
- Analyzed each cluster to identify key characteristics, including demographics, financial behavior, and engagement levels.
- Provided insights into the behavior and preferences of each customer segment.

## Marketing Strategies
- Developed personalized marketing strategies tailored to each identified segment to enhance engagement and increase subscriptions to term deposits.

## Conclusion
The project successfully identified four customer segments, providing valuable insights that can be leveraged for targeted marketing campaigns. The personalized strategies developed aim to meet the unique needs of each segment, driving customer satisfaction and retention.





