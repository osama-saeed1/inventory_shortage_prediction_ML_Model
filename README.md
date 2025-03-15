# Predicting Impending Inventory Shortages Using Machine Learning

In this project, I developed a machine learning model aimed at predicting impending inventory shortages based on a variety of key parameters. This was a binary classification instance where the model predicts whether items will go on backorder (yes or no). The dataset used for this project was extracted from [Kaggle](https://www.kaggle.com/datasets/gowthammiryala/back-order-prediction-dataset) and includes data related to national inventory levels, lead times, quantities in transit, and various sales forecasts over different time frames. Specifically, the parameters included in the analysis are:

- **National Inventory (national_inv)**: The total inventory available at a national level.
- **Lead Time (lead_time)**: The time taken for inventory to be replenished.
- **In-Transit Quantity (in_transit_qty)**: The amount of inventory currently in transit.
- **Forecasts**: Sales forecasts for 3, 6, and 9 months (forecast_3_month, forecast_6_month, forecast_9_month).
- **Sales Data**: Historical sales data for 1, 3, 6, and 9 months (sales_1_month, sales_3_month, sales_6_month, sales_9_month).
- **Minimum Bank (min_bank)**: The minimum inventory level that should be maintained.
- **Potential Issues (potential_issue)**: Any potential issues that could affect inventory levels.
- **Pieces Past Due (pieces_past_due)**: The number of items that are overdue for delivery.
- **Performance Metrics**: Average performance over 6 and 12 months (perf_6_month_avg, perf_12_month_avg).
- **Local Backorder Quantity (local_bo_qty)**: The quantity of items on backorder at a local level.
- **Risk Factors**: Various risk indicators such as deck risk, OE constraint, PPAP risk, stop auto buy, and revenue stop.

![Screenshot from 2025-03-16 02-12-46](https://github.com/user-attachments/assets/0fae1dc6-0254-4382-94f5-19029bc29ef3)
![Screenshot from 2025-03-16 02-13-31](https://github.com/user-attachments/assets/3de49d3c-c74e-4e84-bcd5-77ed47ffd185)

I utilized Python for the implementation and conducted the work on Google Colab. The model was trained on a dataset comprising 20,000 binary samples (Yes and No), indicating whether items went on backorder. The data was split 90/10 i.e., 90% of the data was used for training and 10% was used for testing

For model training, I employed logistic regression due to its effectiveness in binary classification tasks and its ability to provide interpretable results. Logistic regression is particularly suitable for this project as it estimates the probability of an item going on backorder based on the input features, allowing for clear insights into the factors influencing inventory shortages. After rigorous training and validation, the model achieved an accuracy of 73.67% on the test data.

I utilized libraries such as Pandas for data manipulation, NumPy for numerical operations, and Scikit-learn (sklearn) for model training and evaluation. By leveraging these metrics, the model effectively learns patterns and relationships that signal potential inventory shortages, enabling businesses to proactively manage their stock levels and mitigate the risk of backorders. This predictive capability is crucial for maintaining customer satisfaction and optimizing supply chain operations.

*Please note: The python code is utterly disorganized and reading through it may give you a severe migraine. I am afraid that in the pursuit of making the code appear more professional, the model might cease to work which is partly why I am not going to bother with that, the other reason being that I have no will to do so, as long as the model works.*

<!-- Failed to upload "Training_BOP.csv" -->

<!-- Failed to upload "modified_training_bop (1).csv" -->
