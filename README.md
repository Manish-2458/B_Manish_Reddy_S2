Objective:-
The main aim is to analyse the given dataset and use different pre-processing techniques to enhance a machine learning model.

Data description:-

Number of attributes are 18.
Classification type: Regression.
The attributes of the dataset are as follows:- 
1. ID(Numeric)
2. Price(Numeric)
3. Levy(Numeric)
4. Manufacturer(String)
5. Model(String)
6. Prod. year(Numeric)
7. Category(String)
8. Leather interior(String)
9. Fuel type(String)
10. Engine volume(Numeric)
11. Mileage(Numeric)
12. Cylinders(Numeric)
13. Gear box type(String)
14. Drive wheels(String)
15. Doors(String)
16. Wheel(String)
17. Color(String)
18. Airbags(Numeric)

Procedure:-

1. Firstly, downloaded the dataset from the link(https://www.kaggle.com/datasets/deepcontractor/car-price-prediction-challenge).
2. The imported modules are numpy, pandas,matplotlib.pyplot ans sklearn.preprocessing
3. Loaded the dataset from google.colab by importing "files".
4. After loading the dataset,loaded the dataset into a pandas dataframe for further analysis and processing.
5. Here we are droping the attribute "ID" along with it's column axis, and the dataset is divided into feature(X) and the target variable(y), the features are stored in X, and the corresponding target variable values are stored in y, allowing for the application of machine learning algorithm.
6. Now as the dataset contains strings along with integers used "OrdinalEncoder" to modify the data, firstly created an instance of OrdinalEncoder, then used "fit_transform" method of the OrdinalEncoder class which fits the encoder on the specified columns and then transforms those columns into ordinal-encoded values. 
7. The original cateogorical values are replaced with their corresponding numerical representation.The encoding process assigns a unique numerical label to each unique category within each column, representing the order or rank of the categories.
8. Now, for the following datset we are plotting four graphs for comparision of different features with respect to price.
   - The first graph is a "Pie-chart" of Fuel type vs Price
   - The second graph is a "Bar graph" of Manufacturer vs. Price
   - The third graph is a "Line plot" of Prod. year vs Price
   - The fourth graph is a "Scatter plot" of Engine volume vs Price.
9. The null rows are checked and removed using the function dropna().
10. Standardization, also known as Z-score scaling, it transforms the features of a dataset to zero mean and unit variance. Now the given dataset is standardized using StandardScaler
11. Correlation matrix is calculated using the function corr().

Note:- Inline comments are also mentioned at each part of the code.

