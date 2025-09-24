#  Data Analysis Assignments

This document contains multiple datasets and tasks for students to
practice **Data Cleaning, EDA, Grouping, Filtering, Aggregations, and
Visualization** using **Python (Pandas + Matplotlib/Seaborn)**.

------------------------------------------------------------------------

## Assignment 1 -- Retail Sales Data

### Tasks

1.  **Data Cleaning**
    -   Clean Customer Names:
        -   Remove leading/trailing spaces, special characters (\*, !).
        -   Standardize case (make all lower/upper).
    -   Work with Dates:
        -   Convert Date column to datetime.
        -   Extract Year, Month, Day.
        -   Filter all February orders.
2.  **Check Duplicates**
    -   Detect duplicates in the dataset.
    -   Remove them.
3.  **Handle Missing Values**
    -   Manually introduce a few NaN values before class.
    -   Handle them appropriately.
4.  **Add New Columns**
    -   `Profit = Sales * 0.20`
    -   `Total = Sales * Quantity`
5.  **Grouping & Aggregations**
    -   Total sales by Region.
    -   Average sales by Category.
    -   Maximum quantity sold per Product.
    -   Total sales by Region & Category.
6.  **Multiple Aggregations**
    -   For each region → get sum of Sales and mean of Quantity.
7.  **Sorting**
    -   Sort by Sales (highest first).
    -   Sort by Date (oldest first).
8.  **String Filtering**
    -   Get all customers whose name contains "a" (case-insensitive).
9.  **Monthly Sales Trend**
    -   Show total sales per month using `.dt.month_name()`.

------------------------------------------------------------------------

##  Assignment 2 -- Restaurant Sales Data

**Dataset:** `restaurant_sales_1200.csv`

### Tasks

1.  **Data Cleaning**
    -   Remove leading/trailing whitespaces in `Customer` and
        `MenuItem`.
    -   Remove special characters (like \*, !).
    -   Standardize Region names (all lowercase).
2.  **Handling Dates**
    -   Convert `Date` column to datetime format.
    -   Extract Year, Month, Day.
    -   Filter and display all orders from **March 2023**.
3.  **Missing Values**
    -   Detect missing values in the dataset.
    -   Fill missing `Quantity` with the average quantity.
    -   Fill missing `Price` with median price.
4.  **Duplicates**
    -   Check for duplicate rows.
    -   Drop duplicates if any.
5.  **New Columns**
    -   `Total = Quantity * Price`
    -   `Profit = Total * 0.25`
6.  **Grouping & Aggregations**
    -   Total sales per Region.
    -   Average sales per Category.
    -   Top 5 MenuItems by Sales.
    -   Group by Region & Category → show total sales.
7.  **Multiple Aggregations**
    -   For each Region, calculate:
        -   Total Sales
        -   Average Quantity
        -   Maximum Profit
8.  **Sorting**
    -   Sort by Sales (highest first).
    -   Sort by Date (oldest first).
9.  **String Filtering**
    -   Get all customers whose names contain "a".
    -   Get all MenuItem names containing "Pizza".
10. **Monthly Sales Trend**
    -   Show total sales per month using `.dt.month_name()`.
    -   Find the month with the **highest sales**.
11. **Pivot Tables & Crosstabs**
    -   Create a pivot table of Total Sales by Region & Category.
    -   Create a crosstab of MenuItem vs Region (counts of orders).
12. **Exporting Results**
    -   Export the cleaned dataset to CSV and Excel.
    -   Save pivot table results in Excel.
13. **Visualization**
    -   Bar chart → total sales per Region.
    -   Line chart → monthly sales trend.
    -   Bar chart → top 5 MenuItems by Sales.

------------------------------------------------------------------------

##  Assignment 3 -- Cricket Player Performance

### Tasks

1.  **Data Cleaning**
    -   Check for missing values (`isnull()`).
    -   Standardize player names (remove spaces, special characters).
    -   Convert `Match_Date` column to datetime.
    -   Ensure numeric columns
        (`Runs, Balls_Faced, Wickets, Overs_Bowled`) are correct
        datatypes.
2.  **Exploratory Data Analysis (EDA)**
    -   Find total number of players in the dataset.
    -   Top 5 highest run scorers overall.
    -   Top 5 wicket takers overall.
    -   Calculate average runs per player.
    -   Find the player with the highest strike rate (Runs per 100
        balls).
3.  **Grouping & Aggregations**
    -   Total runs scored per country.
    -   Average wickets taken by bowlers per country.
    -   Total matches played by each player role (Batsman, Bowler,
        All-rounder, Wicketkeeper).
    -   Group by Year → total runs and wickets each year.
4.  **Filtering & Sorting**
    -   Get all records where a player scored more than 100 runs.
    -   Find matches where a bowler took 4+ wickets.
    -   Sort players by total runs (descending).
    -   Sort bowlers by best economy rate (`Runs / Overs`).
5.  **String & Date Operations**
    -   Extract Year, Month, Day from `Match_Date`.
    -   Find all matches played in **World Cup 2019 (2019-05 to
        2019-07)**.
    -   Get all players whose name contains "Virat".
6.  **Advanced Tasks**
    -   Create new column `Strike_Rate = (Runs / Balls_Faced) * 100`.
    -   Create new column `Economy_Rate = Runs / Overs_Bowled`.
    -   Find top 5 all-rounders (Runs \> 500 and Wickets \> 20).
    -   Plot monthly run trends for top 3 batsmen.
    -   Bar chart → Total runs by country.

------------------------------------------------------------------------

##  Assignment 4 -- Hospital Patient Data

### Tasks

1.  **Data Cleaning**
    -   Handle missing `Age`, `Gender`, or `Cost`.
    -   Standardize Doctor and Patient names.
2.  **Exploratory Data Analysis (EDA)**
    -   Average age per department.
    -   Total patients by department.
    -   Total and average hospital cost per department.
3.  **Filtering & Sorting**
    -   Patients older than 60.
    -   Patients with stay duration \> 10 days.
    -   Sort patients by `Cost` (descending).
4.  **Grouping & Aggregation**
    -   Total cost per Doctor.
    -   Average stay duration per Department.
    -   Count of follow-ups required per Department.
5.  **Visualization**
    -   Histogram of patient ages.
    -   Pie chart of patients per Department.
    -   Box plot of hospital costs by RoomType.
    -   Stacked bar chart of patients per Department by Gender.
    -   Line chart showing monthly admissions trend.
6.  **Advanced Tasks**
    -   Create new column:
        `StayDuration = DischargeDate - AdmissionDate`.
    -   Find patients with highest cost per Department.
    -   Seaborn heatmap → correlation between Age, Cost, StayDuration.

------------------------------------------------------------------------

##  Deliverables

-   Cleaned dataset.
-   All answers in Python code (**Pandas + Matplotlib/Seaborn**).
-   Visualizations where required.
