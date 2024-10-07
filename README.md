# Car Price Prediction Analysis

## Project Overview
Geely Auto, a prominent Chinese automobile manufacturer, aims to establish a foothold in the US market by setting up a local manufacturing unit. To effectively compete with established US and European car manufacturers, Geely Auto has commissioned a comprehensive analysis to identify the factors influencing car prices in the American market.

## Dataset Description
The dataset used for this analysis encompasses a variety of attributes collected from multiple market surveys across the American market. Key attributes include:

- **Car_ID**: Unique identifier for each observation
- **Symboling**: Assigned insurance risk rating
- **CarCompany**: Manufacturer's name
- **FuelType**: Type of fuel used
- **Aspiration**: Type of aspiration used in the car
- **DoorNumber**: Number of doors in the car
- **CarBody**: Body type of the car
- **DriveWheel**: Type of drive wheel
- **EngineLocation**: Location of the car's engine
- **Wheelbase**: Distance between the centers of the front and rear wheels
- **CarLength**: Length of the car
- **CarWidth**: Width of the car
- **CarHeight**: Height of the car
- **CurbWeight**: Weight of the car without occupants or luggage
- **EngineType**: Type of engine
- **CylinderNumber**: Number of cylinders in the car
- **EngineSize**: Size of the engine
- **FuelSystem**: Type of fuel system
- **BoreRatio**: Bore ratio of the engine
- **Stroke**: Stroke or volume inside the engine
- **CompressionRatio**: Compression ratio of the engine
- **Horsepower**: Engine horsepower
- **PeakRPM**: Maximum revolutions per minute (RPM) of the engine
- **CityMPG**: Mileage in the city
- **HighwayMPG**: Mileage on the highway
- **Price**: Price of the car (dependent variable)

## Project Objectives
1. **Identify Significant Variables**: Determine which variables are significant in predicting car prices.
2. **Analyze Variable Impact**: Assess how well these variables describe car prices.

## Methodology

### Step 1: Data Understanding
- Initial exploration of dataset dimensions, data types, and missing values.
- Descriptive statistics to understand data distribution and summary.

### Step 2: Data Cleaning
- Extract and correct company names from the CarName attribute.
- Handle missing values and remove duplicates.
- Encode categorical variables and scale numerical features for model training.

### Step 3: Exploratory Data Analysis (EDA)
- Visualize the price distribution using histograms and box plots.
- Transform the price variable for normality.
- Examine linear relationships between price and numerical variables.
- Assess multicollinearity among independent variables.

### Step 4: Feature Selection
- Implement forward and backward feature selection using SequentialFeatureSelector.
- Analyze the Variance Inflation Factor (VIF) to detect multicollinearity.

### Step 5: Model Building
- Split the dataset into training and testing sets.
- Build a base model using Linear Regression and update performance metrics in a scorecard.
- Perform hyperparameter tuning for Ridge, Lasso, ElasticNet, Decision Tree, and Random Forest Regressors to identify the best performing model.

### Step 6: Model Evaluation
- Evaluate model performance using metrics such as R² Score, RMSE, and MAPE.
- Select the final model based on evaluation metrics and business understanding.

## Key Findings
- **Significant Variables**: Variables such as wheelbase, engine size, stroke, peak RPM, company name, aspiration turbo, and engine location (rear) significantly impact car prices.
- **Model Performance**: The RandomForestRegressor emerged as the best-performing model, achieving the highest R² score and the lowest RMSE and MAPE on both training and test sets, indicating accurate predictions for the dataset.

## Conclusion
This analysis provides valuable insights for Geely Auto to understand the factors influencing car prices in the US market. By focusing on the identified significant variables, Geely Auto can strategically position their products to compete effectively in the American market.
