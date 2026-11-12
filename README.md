# Ex.-1-Lab-Experiment-Plot-a-Time-Series-Data

## Name: TAMIL MARUDHU K

## Roll no: 2305001033

## Department: CSE

## AIM

To develop a Python program to plot and visualize time series data such as population, commodity market price, or temperature.

## PROGRAM

### 1. Annual Population — 2015–2025

```python
import pandas as pd
import matplotlib.pyplot as plt

year = [2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024, 2025]

population = [90, 93, 96, 98, 100, 103, 106, 110, 114, 118, 123]

data = pd.DataFrame({
    "Year": year,
    "Population": population
})

print(data)

plt.plot(data["Year"], data["Population"])
plt.title("Annual Population")
plt.xlabel("Year")
plt.ylabel("Population (Millions)")
plt.show()
```

### 2. Monthly Temperature — 12 Months

```python
import pandas as pd
import matplotlib.pyplot as plt

month = ["Jan", "Feb", "Mar", "Apr", "May", "Jun",
         "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]

temperature = [25, 27, 30, 33, 35, 34, 32, 31, 30, 29, 27, 25]

data = pd.DataFrame({
    "Month": month,
    "Temperature": temperature
})

print(data)

plt.plot(data["Month"], data["Temperature"])
plt.title("Monthly Temperature")
plt.xlabel("Month")
plt.ylabel("Temperature (°C)")
plt.show()
```

### 3. Monthly Commodity Price — 12 Months

```python
import pandas as pd
import matplotlib.pyplot as plt

month = ["Jan", "Feb", "Mar", "Apr", "May", "Jun",
         "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]

price = [4200, 4350, 4280, 4500, 4650, 4800,
         4700, 4900, 5000, 5150, 5050, 5300]

data = pd.DataFrame({
    "Month": month,
    "Price": price
})

print(data)

plt.plot(data["Month"], data["Price"])
plt.title("Monthly Commodity Market Price")
plt.xlabel("Month")
plt.ylabel("Price")
plt.show()
```

## OUTPUT

### 1. Annual Population — 2015–2025

<img width="929" height="846" alt="image" src="https://github.com/user-attachments/assets/a3abeac0-c0d9-4e8a-a487-7006e8c4742e" />


### 2. Monthly Temperature — 12 Months

<img width="921" height="870" alt="image" src="https://github.com/user-attachments/assets/7873a0b8-3bef-4c64-8257-8ba05862ff9f" />


### 3. Monthly Commodity Price — 12 Months

<img width="921" height="870" alt="image" src="https://github.com/user-attachments/assets/ae5f6d72-35fd-455e-9081-04b23fe7dce4" />


## RESULT

Thus, the given time-series data were successfully stored using Pandas and visualized using Matplotlib. The trends in population, temperature, and commodity price were identified from the plotted graphs.
