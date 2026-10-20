# E-Commerce-Laptop-Price-Prediction-Model
1. Reason Behind Choosing This Project:
   The primary reason I chose this project is because pricing dynamics in e-commerce change rapidly based on original MRPs, customer ratings, and review metrics. As a data science fresher, I wanted a project that deals with structured transactional data, missing values, and numerical regression. E-commerce pricing optimization is a real-world problem faced by platforms like Flipkart and Amazon, making it a very practical portfolio choice.
   
How It Helps the Business:
3. Dynamic Pricing & Competitor Analysis: It helps e-commerce platforms automatically suggest optimal selling prices based on market ratings and original prices.Revenue Optimization: By understanding how customer ratings and discounts impact final sales prices, businesses can strategize discounts better to maximize profit margins.
   
4. Automated Cataloging: It eliminates manual price estimation for new product listings.

Step-by-Step Technical Execution:

Step 1: Data Collection & CombinationI collected multi-date transactional CSV datasets containing laptop listings from e-commerce platforms.Using Python and Pandas, I wrote a script to combine multiple daily CSV files into a single unified DataFrame containing over 9,000 rows.

Step 2: Data Cleaning & Preprocessing
The raw data had missing values and text-formatted pricing attributes.I cleaned the dataset by dropping null rows, converting string prices and ratings into proper numeric data types (pd.to_numeric), and handling outliers to ensure high data quality.

Step 3: Feature Selection & Train-Test Split
I selected key predictive features (original price, total ratings, and customer rating) as independent variables ($X$) and the offer price as the target variable ($y$).I split the dataset into an 80-20 training and testing ratio using Scikit-Learn's train_test_split to prevent model overfitting.

Step 4: Model Training (Machine Learning)
I chose the Random Forest Regressor ensemble algorithm because it handles non-linear relationships and tabular data exceptionally well.I trained the model on the training dataset (model.fit(X_train, y_train)).

Step 5: Model Evaluation & ResultsFinally, I evaluated the model on unseen test data using $R^2$ Score and Mean Squared Error (MSE).The model achieved an outstanding $R^2$ Score of approximately 0.989 (98.9% accuracy), proving that it could accurately predict laptop prices based on the given features.
