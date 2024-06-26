Customer churn is when customers stop using a company's products or services, leading to lost revenue. It happens for reasons like dissatisfaction, better offers elsewhere, or changing needs. Understanding and reducing churn is vital for businesses to retain customers, increase revenue, and improve profitability.
In this project, I took the Telco dataset from Kaggle (https://www.kaggle.com/datasets/blastchar/telco-customer-churn) and performed some tasks as follows:
1. EDA: This gave me some idea about the dataset like how the dataset is and what all insights can I get from it.
2. Preprocessing: Removed the customerID column becasue it was not important to predict the churn rate. Some columns contained only 'yes' and 'no', so I converted them into 1 and 0 and performed one-hot encoding using get_dummies function on some of the columns.
3. Used Logistic Regression and computed the accuracy (~79%), Decision Tree Classifier (~70%). Used GridSearchCV on top of Decision Tree Classifier algorithm to find the best parameters. Apparently, it increased accuracy: (training: ~79%) and (testing: ~77%).
4. Lastly, I tried to use ANN using only one input and output layer with 100 epochs and layered it with early stopping with paramters. Acheived best accuracy in 39th epoch of ~81% in training, ~78% in evaluation and ~78% in testing.
5. I also created a dashboard using Power BI.


Tried Azure ML by providing the preprocessed data and following screenshot will show the result.
<img width="1464" alt="Screenshot 2024-03-20 at 1 11 16 PM" src="https://github.com/Jaggi0504/Telco-Customer-Churn/assets/44519331/b10ee7ca-4e06-4c33-b2db-a4a833fd95fc">

Visulization using Power BI
<img width="869" alt="Screenshot 2024-04-08 at 9 14 09 PM" src="https://github.com/Jaggi0504/Telco-Customer-Churn/assets/44519331/7c20c36d-e794-4110-ac31-25a6b9dc905d">

Visualzing using Excel- Used Pivot charts and slicers for filtering the data after data transformation.
<img width="1470" alt="ExcelScreenshot" src="https://github.com/Jaggi0504/Telco-Customer-Churn/assets/44519331/d1124403-6062-448a-a09a-4acafe5c18b3">
