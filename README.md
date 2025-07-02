📊 GRC Data Dashboard & Analysis (R Shiny)
This project is an interactive data analytics dashboard built in R using Shiny, Plotly, Dplyr, and Arules. It allows users to explore, visualize, and analyze sales data from a CSV file (grc.csv), supporting clustering, association rule mining, and various interactive plots.

🧩 Features
📈 Data Visualization
Pie Chart - Visualizes the distribution of payment types (cash, credit).

Scatter Plot - Shows the relationship between age and total spending.

Bar Plot - Compares total spending across different cities (in descending order).

Box Plot - Displays the distribution of total spending.

🔍 Clustering
Groups customers based on total spending and age using K-means clustering.

User can set the number of clusters dynamically from the interface.

🧠 Association Rules
Uses the Apriori algorithm from the arules package.

Users can specify:

Support

Confidence

Minimum Rule Length

The system dynamically mines and displays association rules based on items purchased.

🛠️ Technologies Used

Shiny (for GUI and interactivity)

Plotly (for interactive charts)

Dplyr (for data wrangling)

Arules (for market basket analysis)

📂 Dataset Requirements
Input file: grc.csv

Required columns:

paymentType: Type of payment (e.g., cash or credit)

total: Total transaction value

age: Customer age

city: Customer city

customer: Customer ID

items: Items in a transaction (comma-separated)

Make sure the file is located at:
C:/Users/PC/Desktop/grc.csv
⚠️ You can change this path inside the script depending on your file location.

🚀 How to Run
Step 1: Install Dependencies
install.packages("shiny")
install.packages("plotly")
install.packages("reader")
install.packages("dplyr")
install.packages("arules")
Step 2: Run the App
library(shiny)
runApp("path/to/your_app_directory")
🖼️ Dashboard Preview
Visualization	Description
Pie Chart	Payment type distribution
Scatter Plot	Age vs Total Spending
Bar Plot	Spending by City
Box Plot	Spending distribution
Clustering Plot	Customer segments
Association Rules	Frequent item patterns
