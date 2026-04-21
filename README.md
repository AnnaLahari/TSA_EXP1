# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 20-04-2026

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
from matplotlib import pyplot as plt
import pandas as pd
df['date']=pd.to_datetime(df['date'], format='mixed')
df.dtypes
df.set_index('date',inplace=True)
df_resampled = df['transaction_amount'].resample('D').sum().interpolate()
df_resampled.plot(kind='line',label='Total Sales', color='black')
plt.title('Daily Transaction Amount Over Time') # Updated title for clarity
plt.xlabel('order_id')
plt.ylabel( 'Transaction Amount')
plt.legend()
plt.grid(True)
plt.show()
```
# OUTPUT:

<img width="1326" height="255" alt="image" src="https://github.com/user-attachments/assets/99793da9-6e17-42d1-b676-b0f705e604ff" />

<img width="767" height="607" alt="image" src="https://github.com/user-attachments/assets/761ea719-8789-4cd2-8447-03b4275324ff" />

# RESULT:
Thus we have created the python code for plotting the time series of given data.
