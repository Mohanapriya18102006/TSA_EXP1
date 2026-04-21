# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 21-04-2026

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

# Load dataset
df = pd.read_csv("temperateure_data.csv")

# Convert Date column to datetime
df['Date'] = pd.to_datetime(df['Date'])

# Plot
plt.figure()
plt.plot(df['Date'], df['Temperature'], marker='o')

# Labels
plt.xlabel("Date")
plt.ylabel("Temperature")
plt.title("Time Series Plot")

# Rotate x-axis labels for clarity
plt.xticks(rotation=45)

# Grid
plt.grid()

# Show plot
plt.show()
```











# OUTPUT:

<img width="912" height="766" alt="Screenshot 2026-04-20 215227" src="https://github.com/user-attachments/assets/dfaf03f3-3ffb-4dff-af3e-1d4b4e29232d" />







# RESULT:
Thus we have created the python code for plotting the time series of given data.
