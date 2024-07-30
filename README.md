# Netflix-Data-Cleaning-and-Analysis
![image](https://github.com/user-attachments/assets/8d1371d3-fe5e-4d76-b9e4-b5fb7cb561dd)

## Project Overview
This project involves the cleaning and analysis of the Netflix dataset, which contains information about various shows and movies available on the streaming platform. The dataset includes columns such as show ID, type, title, director, cast, country, date added, release year, rating, duration, listed in (genres), and description. The main objectives of this project are to clean the dataset by handling missing values, transforming data types, and extracting insights through visualizations.
## Worklow
![image](https://github.com/user-attachments/assets/b6ff3d11-641a-44ed-a434-45a03e133f0f)

## Dataset
The dataset used in this project is netflix_titles.csv, which consists of 8807 rows and 12 columns.

## Libraries Used
The following libraries were used in this project:

numpy
pandas
seaborn
matplotlib
warnings

## Data Cleaning 
![image](https://github.com/user-attachments/assets/fc145a1e-4429-4896-bdb2-e41e1906255a)


The dataset is loaded using pandas’ read_csv function.
Data Overview:

Display the first few rows using df.head().
Display the data types and non-null counts using df.info().
Generate summary statistics using df.describe().
Check for missing values using df.isnull().sum().sort_values(ascending=False).
Handling Missing Values:

Replace missing values with the mode of the respective column for columns with missing values: director, cast, country, date_added, rating, and duration.
Check for Duplicates:

Ensure there are no duplicate show_id values using df[‘show_id’].duplicated().sum().
Data Type Transformation:

Convert the date_added column to datetime format using pd.to_datetime(df[‘date_added’], errors=‘coerce’).
Feature Engineering:

## Data Analysis and Insights
![image](https://github.com/user-attachments/assets/4213c7d5-fd2e-47f7-90d0-e5ab63880f28)

1)Distribution of Content Added Each Month:

![image](https://github.com/user-attachments/assets/857128ef-c142-44b4-80bb-e176d7be0f93)

2)Top 5 Countries with Most Content:

![image](https://github.com/user-attachments/assets/e4296392-1c07-49b0-b6f9-a43b80329a92)

## Project Files
netflix_titles.csv: The dataset used for analysis.
Netflix_Data_Cleaning_Analysis.ipynb: Jupyter notebook containing the data cleaning and analysis steps

## Conclusion
The project successfully cleaned the Netflix dataset by handling missing values, transforming data types, and extracting insightful visualizations. The analysis provided insights into the distribution of content added each month, the top countries producing Netflix content, and the overall distribution of content by country.

## Contact
For any questions or suggestions, please contact Utkarsh Singh at 23mb0068@iitism.ac.in.
