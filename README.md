# Auto Analytics: Exploring Car Market Dynamics
This project conducts Exploratory Data Analysis (EDA) on a dataset containing information about cars. It covers various aspects of data preprocessing, visualization, and analysis to derive insights into the characteristics and trends of the cars.

## Table of Contents
- Introduction
- Steps
- Importing Libraries
- Loading Data and Data Understanding
- Data Cleaning
- Detecting Outliers
- Visualization

## Introduction
This project aims to explore and analyze a dataset related to cars, uncovering insights into various attributes such as price, horsepower, and cylinders. By performing EDA, we gain a deeper understanding of the dataset and its underlying patterns.

## Steps
1. Importing Libraries
    - Pandas: Used for data manipulation and analysis.
    - NumPy: Utilized for numerical computations.
    - Seaborn: Employed for data visualization.
    - Matplotlib: Utilized for creating plots and charts.
  
2. Loading Data and Data Understanding
    - The "cars_data.csv" file is loaded into a pandas DataFrame (df).
    - The first and last five rows (df.head(5), df.tail(5)) are displayed to get a glimpse of the data structure.
    - Basic data information (df.info()) is explored, including data types (df.dtypes) and descriptive statistics (df.describe()).

3. Data Cleaning
- Irrelevant columns ('Engine Fuel Type', 'Market Category', etc.) are dropped (df.drop(...)).
- Column names are made more descriptive (df.rename(...)).
- Duplicate rows are identified (duplicate_rows_df) and removed (df.drop_duplicates()).
- Missing values (df.isna().sum()) are examined and dropped (df.dropna()).
  
4. Detecting Outliers
    - Boxplots are generated (sns.boxplot(...)) to visualize potential outliers in columns like price and horse power.
    - Interquartile Range (IQR) is calculated to define outlier thresholds.
    - Rows with values outside the outlier range (IQR) are removed.
      
5. Visualization
- A bar chart (plt.bar(...)) shows the distribution of car makes.
- A heatmap (sns.heatmap(...)) visualizes correlations between numerical features.
- A scatter plot (plt.scatter(...)) explores the relationship between horsepower and price.

6. Analysis
- Which type of cars are sold maximum?
- What is the co-relation between price and mileage?
- How many cars are registered?
- Price distribution between registered and non-registered cars.
- What is the car price distribution based on Engine Value?
- Which Engine Type of cars users preferred maximum?
- Establish corelation between all features using heatmap.
- Distribution of Price