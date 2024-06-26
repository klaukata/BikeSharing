# London Bike Sharing Data Cleaning

*stack: python, pandas, zipfile, jupyter*

In my *bikes.ipynb* file, I performed several steps to prepare a Kaggle dataset for visualization:

1. I imported, downloaded all the necessary Python packages required for the data manipulation and visualization tasks.

2. I downloaded the dataset from Kaggle as a ZIP file.

3. Using the `zipfile` library, I extracted the contents of the ZIP file to access the dataset files.

4. I loaded the CSV file into a DataFrame using the `pd.read_csv()` function.

5. Initially, I **renamed** some column names to better suit the visualization tasks that I planned to perform later.

6. I **adjusted the values** in the 'humidity_percentage' column to ensure they fell within the range [0, 1]

7.  I **converted** the numerical codes in the 'season' column to their corresponding season names ('spring', 'summer', 'autumn', 'winter').

8. Similarly, I replaced the numerical values in the 'weather_code' column with descriptive weather descriptions ('clear', 'rainy', 'cloudy', and so on).

9. After realizing that the 'weather_code' column should actually be named 'weather_description' to better reflect its content, I renamed the column accordingly.

10. Finally, I **exported** the modified DataFrame to an Excel file named 'london_bikes_final.xlsx' using the `.to_excel()` method, making it ready for further visualization and analysis.

This step-by-step preparation ensured that the dataset was cleaned, structured, and labeled appropriately for the visualization tasks I planned to undertake downstream.
___
resources:
- [Kaggle: London bike sharing dataset](https://www.kaggle.com/datasets/hmavrodiev/london-bike-sharing-dataset)