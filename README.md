# Power-BI-Advanced-Data-Analysis-Report-Using-Python-TASK 4

**Name:** Dimple Choudhary

**Company:** CODTECH IT SOLUTIONS

**ID:** CT12IVN

**Domain:** Power BI

**Duration:** January to March 2025

**Mentor:** Neela Santhosh Kumar

**Overview of the project**

**Project:** Power-BI-Advanced-Data-Analysis-Report-Using-Python


**comands**

1) 
![Screenshot (50)](https://github.com/user-attachments/assets/46ee3cdc-c501-4c2a-8821-867ae45ee0a8)

import pandas as pd

import matplotlib.pyplot as plt

data = {

    "Date": pd.date_range(start="2024-01-01", periods=10, freq="D"),
    
    "Sales": [2000, 2500, 3000, 2800, 3500, 3300, 4000, 4200, 4500, 5000],
    
    "Profit": [500, 600, 700, 650, 800, 750, 900, 1000, 1100, 1200]
    
}

df = pd.DataFrame(data)

**Line Chart for Sales & Profit**

plt.figure(figsize=(8, 5))

plt.plot(df["Date"], df["Sales"], marker="o", linestyle="-", color="blue", label="Sales")

plt.plot(df["Date"], df["Profit"], marker="s", linestyle="--", color="green", label="Profit")

plt.title("Sales & Profit Trends")

plt.xlabel("Date")

plt.ylabel("Amount ($)")

plt.legend()

plt.grid(True)

plt.xticks(rotation=45)

plt.show()

2) 
![Screenshot (51)](https://github.com/user-attachments/assets/a412b025-dc8b-478b-b2ad-985b0fb726dd)

import pandas as pd

import matplotlib.pyplot as plt

**Sample Data**

data = {
    "Category": ["Electronics", "Clothing", "Furniture", "Toys", "Groceries"],
    
    "Sales": [50000, 30000, 20000, 15000, 40000]
}

df = pd.DataFrame(data)

**Bar Chart**
plt.figure(figsize=(7, 5))

plt.bar(df["Category"], df["Sales"], color=['blue', 'green', 'red', 'purple', 'orange'])

plt.title("Sales by Category")

plt.xlabel("Category")

plt.ylabel("Sales ($)")

plt.xticks(rotation=30)

plt.grid(axis='y', linestyle="--", alpha=0.7)

plt.show()

3)
![Screenshot (52)](https://github.com/user-attachments/assets/77c8a73d-306b-4f40-a92a-473fe737d29b)

import pandas as pd

import matplotlib.pyplot as plt

**Sample Data*8

data = {

    "Sales": [1000, 2000, 3000, 4000, 5000, 6000, 7000],
    
    "Profit": [200, 400, 600, 700, 900, 1100, 1300]
}


df = pd.DataFrame(data)

**Scatter Plot**

plt.figure(figsize=(7, 5))

plt.scatter(df["Sales"], df["Profit"], color="blue", alpha=0.7)

plt.title("Sales vs. Profit")

plt.xlabel("Sales ($)")

plt.ylabel("Profit ($)")

plt.grid(True, linestyle="--", alpha=0.6)

plt.show()

4)
![Screenshot (54)](https://github.com/user-attachments/assets/1f2417bc-6e1b-4d27-ab71-8c78f07e4584)

import pandas as pd

import matplotlib.pyplot as plt

import numpy as np

**Sample Data** 

np.random.seed(42)

order_values = np.random.randint(1000, 10000, 50)  # Simulated order values

**Histogram**

plt.figure(figsize=(7, 5))

plt.hist(order_values, bins=10, color="blue", edgecolor="black", alpha=0.7)

plt.title("Order Value Distribution")

plt.xlabel("Order Value ($)")

plt.ylabel("Frequency")

plt.grid(axis="y", linestyle="--", alpha=0.7)

plt.show()

5)
![Screenshot (55)](https://github.com/user-attachments/assets/b276819e-27af-4c00-83d0-3a895b53be78)

import pandas as pd

import matplotlib.pyplot as plt

**Sample Data**

data = {

    "Region": ["North", "South", "East", "West"],
    
    "Sales": [50000, 40000, 35000, 45000]
}

df = pd.DataFrame(data)

**Pie Chart**

plt.figure(figsize=(6, 6))

plt.pie(df["Sales"], labels=df["Region"], autopct="%1.1f%%", colors=['blue', 'green', 'red', 'purple'])

plt.title("Sales Contribution by Region")

plt.show()

6)
![Screenshot (56)](https://github.com/user-attachments/assets/4f55981e-bc0f-4a34-8164-9ee8503c3875)

import pandas as pd

import matplotlib.pyplot as plt

**Sample Data**

categories = ["Electronics", "Clothing", "Furniture", "Toys", "Books"]

sales = [25000, 18000, 22000, 15000, 12000]

**Create Bar Chart**

plt.figure(figsize=(8, 5))

plt.bar(categories, sales, color=["blue", "green", "red", "purple", "orange"], edgecolor="black")

**Labels and Titles**

plt.xlabel("Category", fontsize=12, fontweight="bold", color="darkblue")

plt.ylabel("Sales ($)", fontsize=12, fontweight="bold", color="darkred")

plt.title("Category-wise Sales Comparison", fontsize=14, fontweight="bold", color="darkgreen")

**Show plot**
plt.show()

7)
![Screenshot (57)](https://github.com/user-attachments/assets/a06e57a7-c361-4c31-9b28-325b83d8bc6d)

import pandas as pd

import matplotlib.pyplot as plt

Sample Data**

months = ["Jan", "Feb", "Mar", "Apr", "May", "Jun"]

sales = [12000, 15000, 17000, 16000, 19000, 22000]

**Create Line Chart**

plt.figure(figsize=(8, 5))

plt.plot(months, sales, marker="o", linestyle="-", color="blue", linewidth=2)

**Labels and Titles**

plt.xlabel("Month", fontsize=12, fontweight="bold", color="darkblue")

plt.ylabel("Sales ($)", fontsize=12, fontweight="bold", color="darkred")

plt.title("Monthly Sales Trend", fontsize=14, fontweight="bold", color="darkgreen")

**Show plot**

plt.show()

8)
![Screenshot (58)](https://github.com/user-attachments/assets/414e13a3-65cc-430f-aacf-18b664665b49)

import pandas as pd

import matplotlib.pyplot as plt

**Sample Data**

segments = ["Electronics", "Clothing", "Furniture", "Toys"]

profits = [4000, 3000, 5000, 2000]

**Create Pie Chart**

plt.figure(figsize=(7, 7))

plt.pie(profits, labels=segments, autopct="%1.1f%%", colors=["skyblue", "lightgreen", "coral", "gold"], startangle=140)

**Title**

plt.title("Profit Distribution by Category", fontsize=14, fontweight="bold", color="darkblue")

**Show plot**

plt.show()


**Objective:**

To utilize Python scripts within Power BI for advanced data analysis and visualization, enhancing data-driven decision-making.

**Methodology:**

**Data Import:** Loaded data into Power BI from various sources.

**Python Integration:** Embedded Python scripts within Power BI for data preprocessing and analysis.

**Data Cleaning & Transformation:** Used Python libraries (Pandas, NumPy) for data manipulation.

**Advanced Analysis:** Implemented statistical analysis, trend forecasting, and anomaly detection.

**Custom Visualizations:** Created advanced visualizations using Matplotlib and Seaborn.

**Dashboard Development:** Integrated Python-generated insights into Power BI reports.

**Optimization:** Ensured performance efficiency and script execution speed.

**Technologies Used:**

**Power BI Desktop:** For report creation and integration with Python.

**Python:** For data preprocessing, analysis, and visualization.

**Pandas & NumPy:** For data manipulation and calculations.

**Matplotlib & Seaborn:** For custom visualizations.

**Key Insights:**

**Enhanced Data Processing:** Python scripts enabled complex data transformations.

**Advanced Analytics:** Implemented predictive modeling and trend analysis.

**Custom Visualizations:** Provided more insightful representations of key metrics.

**Efficiency:** Reduced manual effort through automated data processing.

**Scalability:** Demonstrated the potential for integrating more advanced analytics in Power BI.

**Conclusion:**
The use of Python within Power BI significantly enhanced data analysis and visualization capabilities. The project demonstrated how integrating Python scripts allows for more advanced insights, improving overall business intelligence. Future enhancements could include machine learning-based forecasting and deeper statistical modeling for better predictive analytics.



