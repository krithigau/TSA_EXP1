# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 11-03-2025

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt

# Load the CSV file
file_path = 'AI_Resume_Screening.csv'  
data = pd.read_csv(file_path)
data.set_index('Salary Expectation ($)', inplace=True)

plt.figure(figsize=(15, 6))
plt.title('Salary growth over time')
plt.xlabel('Experience (Years)')
plt.ylabel('Salary Expectation ($)')
plt.plot(data.index, data['Salary Expectation ($)'], label='Salary Expectation', color='violet')
```
# OUTPUT:

![Screenshot 2025-03-11 094257](https://github.com/user-attachments/assets/106480b9-2ade-439a-9e04-5e957812fba1)

# RESULT:
Thus we have created the python code for plotting the time series of given data.
