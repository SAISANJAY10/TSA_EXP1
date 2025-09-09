# Ex.No: 01A PLOT A TIME SERIES DATA

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
import statsmodels.api as sm

data=sm.datasets.sunspots.load_pandas().data

print(data.head())

mean = data["SUNACTIVITY"].mean()
print("Mean Close Price:", mean_close)

plt.plot(data['YEAR'], data['SUNACTIVITY'])
plt.title("Yearly Sunspot Counts")
plt.xlabel("Year")
plt.ylabel("Sunspot Count")
plt.show()

```
# OUTPUT:

<img width="380" height="93" alt="image" src="https://github.com/user-attachments/assets/5c3aa190-535f-4ad4-b014-8565e6d12e3a" />

<img width="764" height="561" alt="image" src="https://github.com/user-attachments/assets/34759c10-be6d-41f2-b876-16ed08680e3b" />

# RESULT:
Thus we have created the python code for plotting the time series of given data.
