# Car_Sales_Analysis_Using_Python

## 1.0. Title
Car Sales Analysis using Python

## 2.0 Introductilon
### 2.1. Objectives: 

The analysis focused on achieving the following:

a) to determine the manufacturer with the highest and lowest average sales volume.

b) to discover the distribution of car prices in the data.

c) to determine how the different numerical variables in the data set correlates with each other.

d) to determine the relationship between price and latest launch year.

e) to group cars by manufacturers in order to analyze their average price and fuel efficiency.

f) to identify and visualize the most popular car brands. g) to identify which car model has the highest resale value compared to its initial price.

h) to find out the top 3 fuel-efficient cars with an engine size above 2.5 liters.

i) to determine which Lexus model has the highest horsepower.

### 2.2. Context:

The dataset the different fields collected by a company that deals on car sales.  Some of the variables that made up the dataset includes: Car Manufacturer, Model, Sales, year resale value, Vehicle type, Price, Engine size, Horsepower, Wheelbase, Width, Length, Curb weight, Fuel capacity, Fuel efficiency, Latest Launch year and Power perf factor. The dataset contains different datatype which includes: strings, integers and floats.

### 2.3. Data Sources

The primary source of data used here is Car_sales.csv and it's an open source data which was given as a practice data. The following is the link to the dataset: 

https://drive.google.com/file/d/1TLTcaj1-YRat32RBeKwl-g3eyUP7QI5u/view?usp=drive_link

## 3.0. Data Understanding

### 3.1. Data description: The dataset came as a structured dataset which contained 157 observations and 16 columns. 

### 3.2. Exploratory data analysis (EDA): 
Python (Jupiter notebook) was implored in cleaning and analyzing the dataset. At the end of the analysis, we were able to determine:

a) the manufacturer with the highest and lowest average sales volume.

b) the distribution of car prices in the dataset.

c) how the different numerical variables in the data set correlates with each other.

d) the relationship between price and latest launch year.

e) the average price and fuel efficiency of each manufacturer by grouping.

f)  the most popular car brands by visualization.

g) which car model has the highest resale value compared to its initial price.

h) the top 3 fuel-efficient cars with an engine size above 2.5 liters.

i) which Lexus model has the highest horsepower.

## 4.0. Methodology
### 4.1. Data preprocessing/Analytical Approach

The dataset was imported into Jupiter notebook, including the different libraries like: numpy, pandas, matplotlib and seaborn. The dataset was called 'data'.

#### Some of the steps taken in the preprocessing of the data are:

a) viewing the dataset to determine the number of rows and columns (data.shape).

b) determining the different data types of the different columns in the dataset (data.info() which data.dtypes worked perfectly for it too) and also changing the columns with 
inappropriate datatypes with the appropriate one.

c) checking for missing values and their number in each column (data.isnull().sum()), filling up the 'year resale value' with it's average (Average_year_sales =data["_year_resale_value"].mean(), data.["_year_resale_value"].fillna, Average_year_sales, inplace= True) and dropping the other rows with null values (data= data.dropna()).

d) cleaning the name of the "__year_resale_value" column by removing the leading underscore (data.rename.(columns={'__year_resale_value:"year_resale_value}, inplace= True))

e) descriptive statistics (mean, median, standard deviation) were conducted on the numerical columns (data.describe()).

f) checking and removing of duplicates from the dataset (data.duplicated().sum())

### 4.2. Assumptions:
Customers preferred cars produced by ‘Ford’ manufacturer compared to those produced by other manufacturers due to its average price and fuel efficiency.

## 5.0. Analysis
### 5.1. Results:

#### Car model with the highest resale value compared to its initial price

![picture 1](https://github.com/user-attachments/assets/ad471307-1f21-4328-84a5-8f89f01185a4)

#### Counting the number of missing values in each column 

![picture 2](https://github.com/user-attachments/assets/e8320966-5b8b-46ed-aa90-67d2083086da)

#### Dropping the columns with null values

![picture 3](https://github.com/user-attachments/assets/09b088c7-a038-4260-8003-88f1e2c21082)

#### Distribution of Car price in the dataset

![picture 4](https://github.com/user-attachments/assets/9209bd83-292b-4ec3-8652-ee0abc0d0ec3)

#### Correlation of numerical values in the dataset

![picture 5](https://github.com/user-attachments/assets/33409225-ba9e-4ad0-84ad-1627f109f63f)

#### Relationship between Price and Latest launch year

![picture 6](https://github.com/user-attachments/assets/c6fe8082-64c6-4364-8f56-41a45c9897c8)

### 5.2. Interpretation/key findings: 

From the result, it can be seen:

•	‘Ford’ is the Manufacturer with the highest average sales volume while ‘Porsche’ is the manufacturer with the lowest average sales volume.

•	‘Mercedes-B’ is the manufacturer with the highest car price in the dataset.

•	There’s a strong correlation between ‘Horsepower’ and ‘Power perf factor’ where p=0.99.

•	The highest increase in Car price was in 2011.

•	‘Ford’ is mostly purchased by customers.

•	Car model with the highest resale value is Carrera Cabrio. 

•	‘Impala’, ‘Monte Carlo’ and ‘CLK Coupe’ are the top three (3) fuel efficient cars with an engine above 2.5 liters.

•	The ‘Lexus’ model with the highest ‘Horsepower’ is ‘Viper’ with 450 Horsepower.

## 6.0. Conclusion
### 6.1. Summary of finding:

•	The dataset came as a structured dataset which contained 157 observations and 16 columns. 

•	The dataset contains integers, strings and floats.

•	The ‘Year resale value’ column had the highest null value (36) in the dataset.

•	The dataset had no duplicates but contains a total of fifty-one (51) null values. 

•	‘Ford’ is the Manufacturer with the highest average sales volume while ‘Porsche’ is the manufacturer with the lowest average sales volume.

•	‘Mercedes-B’ is the manufacturer with the highest car price in the dataset.

•	There’s a strong correlation between ‘Horsepower’ and ‘Power perf factor’ where p=0.99.

•	The highest increase in Car price took place in 2011.

•	‘Ford’ is most popular Car Manufacturer.

•	‘Carrera Cabrio’ is the Car model with the highest resale value.

•	‘Impala’, ‘Monte Carlo’ and ‘CLK Coupe’ are the top three (3) fuel efficient cars with an engine above 2.5 liters.

•	The ‘Lexus’ model with the highest ‘Horsepower’ is ‘Viper’ with 450 Horsepower.

## 7.0. Acknowledgement

I acknowledge PSP ANALYTICS for this great platform for learning. I want to sincerely appreciate our facilitators for providing the dataset that was used for this analysis and for their tireless efforts to ensure we get the best from the training. Google Colab was employed in this analysis.

