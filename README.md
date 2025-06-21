# BigData_Creditcard_fraudDetection_1

** COMPANY **    : CODETECH IT SOLUTIONS

** NAME **       : DUBBIREEDY NARASIMHA KRISHNA CHAITANYA

** INTERN ID **  : CT06DN610

** DOMAIN **     : DATA ANALYSIS

** BATCH DURATION ** : May 15th, 2025 to June 30th, 2025.

** MENTOR NAME **     : NEELA SANTOSH 

** DESCRIPTION **     :  In this task, I worked on analyzing a large dataset of credit card transactions. The main goal was to find patterns that could help in detecting fraudulent transactions. Fraud detection is an important topic in finance because even a small number of fraudulent transactions can cause big losses for companies and customers.

The dataset I used contained about 284,807 records. This means it had information about nearly 285,000 different credit card transactions. Out of these, only a very small portion were actually fraud, and most of them were normal. This kind of situation is called imbalanced data, where one class (normal transactions) has many records and the other class (fraudulent transactions) has very few. Dealing with imbalanced data is one of the key challenges in fraud detection.

Because the dataset was large, I decided to use PySpark, which is a tool that helps process big data very efficiently. Normally, when we work with large datasets on a personal computer, the system may become slow or even crash because of limited memory. But with PySpark, the data is processed in smaller pieces (distributed processing), which makes it much faster and easier to handle.

I started by uploading the data into Google Colab and loaded it into a PySpark DataFrame. The first step was to check the dataset for any missing values or errors. Fortunately, the data was already clean, so I didn’t have to spend much time on data cleaning.

After that, I studied the structure of the data to understand what kind of information it contained. Each transaction had several features (columns), like the amount of money involved in the transaction, time, and some encoded features labeled as V1, V2, V3, etc., which were generated through a technique called PCA (Principal Component Analysis) for privacy reasons.

Next, I analyzed how many transactions were fraudulent and how many were normal. As expected, most transactions were normal, and only a small number were fraud. This helped me understand the scale of the problem that fraud detection systems face — finding the few bad transactions hidden among millions of good ones.

I then applied feature scaling using PySpark’s StandardScaler tool. Scaling is important because some features may have very large values while others have small ones. If we don’t scale the data, the model may pay too much attention to features with larger numbers and ignore the smaller ones, even if they are important. By scaling, all features are brought into a similar range, making the analysis more balanced.

Finally, I used PySpark to quickly summarize the transaction amounts, count how many transactions were fraud vs normal, and observe patterns. For example, I noticed that many fraud transactions involved smaller amounts, which could be a trick used by fraudsters to avoid getting detected easily.

The biggest learning from this task was how powerful tools like PySpark are when working with big data. In real banks and financial companies, millions of transactions happen every day, and they need systems that can process huge amounts of data quickly and accurately. This experience showed me how big data tools can help in such situations, making fraud detection faster and more effective.

In the end, I successfully processed the large credit card transaction data, generated useful insights, and prepared the data for the next tasks like machine learning and visualization.
