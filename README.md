# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 21-04-2026

# AIM:

To Develop a python program to Plot a time series data (population/ market price of a commodity
 temperature.
 
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
df = pd.read_excel("/content/temperature_data.xlsx")

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

<img width="743" height="629" alt="Screenshot 2026-04-21 222555" src="https://github.com/user-attachments/assets/cb6a6d02-8db4-4358-8d30-d25180e9b13a" />







# RESULT:
Thus we have created the python code for plotting the time series of given data.
