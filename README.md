# Housing_prices
Housing prices prediction with XGBoost algorithm. The train and test datasets were obtained from a Kaggle competition. ALl the code is done ina  single Python notebook. The main considerations are:

  (1) We used label encoding to get categorical data into numerical

  (2) We performed feature engineering. We added features related to thetotal square feet of the house, age-related features, luxury features, and most importantly, we classified the neighbourhoods in terms of the meadian price of houses from the training set.

  (3) We implemented a XGBoost model with 1000 estimators (trees) and a learning rate of 0.05.

  (4) To train the model, we use the logarithm of the SalePrice, to account equaly the error of more expensive and cheaper houses.

![image](https://github.com/user-attachments/assets/0615b2ac-2572-4f19-aeb0-2bf47fb5d7c7)

We end up with a decent model that underprices the higher houses in the spectrum. The mean error is of 15.8 K$.

The following plot of the SHAP values shows the most relevant features in the model (features starting with an underscore _ have been added in the feature engineering step)

![image](https://github.com/user-attachments/assets/f74521c6-4e9e-40f7-a34f-ca852c696dbe)
