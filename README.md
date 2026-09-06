# 📊 Pandas Analyzer & Data Visualization

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Python](https://img.shields.io/badge/Python-3.x-yellow)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-green)


### Sales Data Analysis & Visualization System

A Python-based data analysis project developed using **Pandas, NumPy, Matplotlib and Seaborn**.

**Developer:** Chand Khimani  
**Course:** BCA — Final Year  
**Subject:** Data Analysis  
**Guided By:** Girish Gondaliya Sir

</div>

---

## 📌 Project Overview

**Pandas Analyzer & Data Visualization** is a menu-driven Python application designed to analyze and visualize sales data.

The project demonstrates practical implementation of:

- Pandas DataFrame operations
- NumPy array operations
- Data cleaning
- Missing value handling
- Mathematical operations
- Data searching, sorting and filtering
- Aggregation functions
- Statistical analysis
- GroupBy and Transform
- Pivot tables
- DataFrame combining and splitting
- Data visualization
- Object-Oriented Programming
- Exception handling
- Exporting analysis results
- Saving visualizations

The project uses a sample sales dataset containing product, region, sales, profit, year and date information.

---

# 🎯 Project Objectives

The main objectives of this project are:

1. To understand and implement Pandas DataFrame operations.
2. To perform practical sales data analysis.
3. To demonstrate NumPy array conversion, indexing and slicing.
4. To clean and handle missing data.
5. To perform mathematical and statistical operations.
6. To search, sort and filter sales records.
7. To combine and split DataFrames.
8. To use aggregation functions for meaningful analysis.
9. To create pivot tables and perform GroupBy operations.
10. To visualize sales data using Matplotlib and Seaborn.
11. To implement Object-Oriented Programming using a class.
12. To provide a simple menu-driven interface.
13. To save important visualizations and analysis results.

---

# 🏗️ Project Architecture

```text
                    ┌───────────────────────┐
                    │      Sales Dataset    │
                    │      sales_data.csv   │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │   SalesDataAnalyzer   │
                    │        Class          │
                    └───────────┬───────────┘
                                │
          ┌─────────────────────┼─────────────────────┐
          ▼                     ▼                     ▼
   Data Exploration       Data Cleaning        Data Processing
          │                     │                     │
          ▼                     ▼                     ▼
   Statistics             Missing Values       DataFrame Operations
          │                                           │
          └─────────────────────┬─────────────────────┘
                                ▼
                    ┌───────────────────────┐
                    │       Analysis        │
                    │   & Visualization     │
                    └───────────┬───────────┘
                                │
             ┌──────────────────┼──────────────────┐
             ▼                  ▼                  ▼
         Matplotlib          Seaborn           Export
       Visualizations      Visualizations      Results
```

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data Analysis & DataFrame Operations |
| NumPy | Numerical & Array Operations |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Jupyter Notebook | Development Environment |
| Google Colab | Notebook Execution |
| CSV | Dataset Storage |
| GitHub | Project Documentation & Submission |

---

# 📂 Project Structure

```text
PR_9_Pandas_Analyzer/
│
├── Pandas_Analyzer.ipynb
├── sales_data.csv
└── README.md
```

### Files Description

**Pandas_Analyzer.ipynb**  
Contains the complete Python implementation, analysis, operations, visualizations and menu-driven interface.

**sales_data.csv**  
Contains the sales dataset used for analysis.

**README.md**  
Contains complete project documentation.

---

# 📊 Dataset Information

The project uses a synthetic sales dataset created using Python and Pandas.

### Dataset Size

- **Rows:** 20
- **Columns:** 7

### Dataset Columns

| Column | Description |
|--------|-------------|
| SalesID | Unique identifier for each sales record |
| Product | Name of the product |
| Region | Sales region |
| Sales | Sales amount |
| Profit | Profit generated |
| Year | Sales year |
| Date | Sales date |

### Dataset Columns

```text
['SalesID', 'Product', 'Region', 'Sales', 'Profit', 'Year', 'Date']
```

---

# 🔄 Data Processing Workflow

The project follows this workflow:

```text
Load Dataset
     ↓
Explore Dataset
     ↓
Check Missing Values
     ↓
Clean Dataset
     ↓
Convert Data Types
     ↓
NumPy Operations
     ↓
Mathematical Operations
     ↓
Combine / Split Data
     ↓
Search / Sort / Filter
     ↓
Aggregation
     ↓
Statistical Analysis
     ↓
GroupBy / Transform
     ↓
Pivot Table
     ↓
Re-index / Alter Labels
     ↓
Visualization
     ↓
Save Visualization
     ↓
Export Analysis Results
     ↓
Conclusion
```

---

# 🧱 Object-Oriented Programming

The complete analysis functionality is encapsulated inside:

```python
class SalesDataAnalyzer:
```

The class contains the main data analysis and visualization methods.

## Encapsulation

The DataFrame is stored inside the class using:

```python
self.data
```

This allows the dataset and its operations to be managed through the class.

---

# 🔧 Core Methods

The project implements the following important methods:

```text
__init__()
__del__()
load_data()
explore_data()
clean_data()
mathematical_operations()
numpy_operations()
combine_data()
split_data()
search_sort_filter()
aggregate_functions()
statistical_analysis()
create_pivot_table()
groupby_transform()
reindex_and_labels()
dataframe_operations()
visualize_data()
save_visualization()
export_analysis()
conclusion()
```

---

# 🔢 NumPy Operations

Relevant Pandas columns are converted into NumPy arrays using:

```python
sales_array = self.data["Sales"].to_numpy()
```

The project demonstrates:

### Array Conversion

```python
sales_array = self.data["Sales"].to_numpy()
```

### Indexing

```python
sales_array[0]
```

### Slicing

```python
sales_array[:5]
```

and:

```python
sales_array[2:7]
```

This demonstrates practical NumPy array indexing and slicing.

---

# ➕ Mathematical Operations

Element-wise mathematical operations are performed on the sales dataset.

### 10% Sales Increase

```python
self.data["Sales_With_10_Percent_Increase"] = (
    self.data["Sales"] * 1.10
)
```

### Sales-Profit Difference

```python
self.data["Sales_Profit_Difference"] = (
    self.data["Sales"] - self.data["Profit"]
)
```

These operations demonstrate mathematical calculations directly on DataFrame columns.

---

# 🔗 Combining DataFrames

Multiple DataFrames can be combined using Pandas `concat()`.

```python
combined_data = pd.concat(
    [self.data, other_dataframe],
    ignore_index=True
)
```

This demonstrates combining multiple datasets into a single DataFrame.

---

# ✂️ Splitting Data

The dataset can be split based on:

- Region
- Product

The project uses `groupby()` to create separate DataFrames.

Example:

```python
for value, group in self.data.groupby("Region"):
    split_dataframes[value] = group.copy()
```

Each group represents a separate section of the dataset.

---

# 🔎 Search, Sort & Filter

The project demonstrates different DataFrame selection techniques.

## Product Search

Products containing a specific keyword can be searched.

```python
self.data[
    self.data["Product"].str.contains(
        "Lap",
        case=False,
        na=False
    )
]
```

## Sorting

Sales records are sorted from highest to lowest:

```python
self.data.sort_values(
    by="Sales",
    ascending=False
)
```

## Region Filtering

```python
self.data[
    self.data["Region"] == "North"
]
```

## Year Filtering

```python
self.data[
    self.data["Year"] == 2025
]
```

---

# 📈 Aggregate Functions

The project uses Pandas aggregation functions such as:

- `sum()`
- `mean()`
- `count()`

### Total Sales

```python
self.data["Sales"].sum()
```

### Average Sales

```python
self.data["Sales"].mean()
```

### Total Profit

```python
self.data["Profit"].sum()
```

### Average Profit

```python
self.data["Profit"].mean()
```

### Number of Records

```python
self.data["Sales"].count()
```

### Sales by Region

```python
self.data.groupby("Region")["Sales"].agg(
    ["sum", "mean", "count"]
)
```

---

# 📊 Statistical Analysis

The project performs descriptive statistical analysis using Pandas.

## Descriptive Statistics

```python
self.data[["Sales", "Profit"]].describe()
```

The `describe()` function provides:

- Count
- Mean
- Standard Deviation
- Minimum
- 25th Percentile
- Median
- 75th Percentile
- Maximum

## Standard Deviation

```python
self.data[["Sales", "Profit"]].std()
```

## Variance

```python
self.data[["Sales", "Profit"]].var()
```

## Percentiles

```python
self.data[["Sales", "Profit"]].quantile(0.25)
```

```python
self.data[["Sales", "Profit"]].quantile(0.50)
```

```python
self.data[["Sales", "Profit"]].quantile(0.75)
```

---

# 📌 Pivot Table

The project creates a sales pivot table based on Region and Product.

```python
pivot = pd.pivot_table(
    self.data,
    values="Sales",
    index="Region",
    columns="Product",
    aggfunc="sum",
    fill_value=0
)
```

This helps compare product sales across different regions.

---

# 🔄 GroupBy & Transform

The project demonstrates `groupby()` with `transform()`.

```python
self.data["Region_Average_Sales"] = (
    self.data.groupby("Region")["Sales"]
    .transform("mean")
)
```

This calculates the average sales of each region and adds the result to every corresponding record.

---

# 🔤 Re-indexing & Altering Labels

The project demonstrates changing DataFrame index labels.

```python
sample_data = self.data.head(5).copy()

sample_data.index = [
    "Record_A",
    "Record_B",
    "Record_C",
    "Record_D",
    "Record_E"
]
```

This demonstrates how DataFrame index labels can be customized.

---

# 📊 Data Visualization

The project provides multiple visualization options using Matplotlib and Seaborn.

### Matplotlib Visualizations

- Bar Chart
- Line Chart
- Scatter Plot
- Pie Chart
- Histogram
- Stack Plot

### Seaborn Visualizations

- Heatmap
- Box Plot

### Additional

- Subplots

---

# 📊 1. Bar Chart

The Bar Chart represents total sales by product.

```text
Product → Sales
```

It helps identify which products generate higher sales.

---

# 📈 2. Line Chart

The Line Chart represents yearly sales trends.

```text
Year → Total Sales
```

It helps understand changes in sales across different years.

---

# 🔵 3. Scatter Plot

The Scatter Plot represents:

```text
Sales vs Profit
```

It helps visualize the relationship between sales and profit.

---

# 🥧 4. Pie Chart

The Pie Chart represents sales distribution by region.

```text
Region → Sales Percentage
```

It provides a simple view of regional contribution to total sales.

---

# 📊 5. Histogram

The Histogram represents the distribution of sales values.

It helps understand how frequently different sales values occur.

---

# 📚 6. Stack Plot

The Stack Plot represents regional sales over different years.

```text
Year → Regional Sales
```

It helps compare the contribution of different regions over time.

---

# 🔥 Seaborn Visualizations

## Heatmap

The project creates a correlation heatmap using:

```python
sns.heatmap(
    numeric_data.corr(),
    annot=True,
    cmap="coolwarm"
)
```

The heatmap helps identify relationships between numerical columns such as:

- Sales
- Profit
- Year

---

# 📦 Box Plot

A Seaborn Box Plot is used to display sales distribution by region.

```python
sns.boxplot(
    data=self.data,
    x="Region",
    y="Sales"
)
```

It helps compare sales distributions across different regions.

---

# 🖼️ Subplots

The project also demonstrates multiple charts in a single figure.

Example:

```text
┌─────────────────────┬─────────────────────┐
│   Sales by Product  │    Sales vs Profit  │
│                     │                     │
│      Bar Chart      │    Scatter Plot     │
└─────────────────────┴─────────────────────┘
```

This provides a compact visual comparison.

---

# 💾 Saving Visualizations

Important visualizations can be saved using:

```python
self.current_plot.savefig(
    file_name,
    dpi=300,
    bbox_inches="tight"
)
```

The project supports saving visualizations as image files such as:

```text
PNG
JPEG
```

---

# 📤 Exporting Analysis Results

The project can export important analysis results into a CSV file.

Example output:

```text
analysis_results.csv
```

The exported file contains metrics such as:

```text
Total Sales
Average Sales
Total Profit
Average Profit
```

---

# 🧹 Data Cleaning & Missing Values

The project checks for missing values using:

```python
self.data.isnull().sum()
```

Numeric missing values are handled using the mean of the respective column.

```python
self.data[column] = self.data[column].fillna(
    self.data[column].mean()
)
```

The project also demonstrates missing-value options through the menu system:

1. Display rows with missing values
2. Fill missing values with mean
3. Drop rows
4. Replace missing values with a specific value

---

# 🔄 Data Type Conversion

During dataset loading, important columns are converted into suitable data types.

### Date Conversion

```python
self.data["Date"] = pd.to_datetime(
    self.data["Date"],
    errors="coerce"
)
```

### Numeric Conversion

```python
self.data[column] = pd.to_numeric(
    self.data[column],
    errors="coerce"
)
```

This helps maintain correct data types for analysis.

---

# ⚠️ Exception Handling

The project uses exception handling while loading the dataset.

Example:

```python
try:
    self.data = pd.read_csv(file_path)

except FileNotFoundError:
    print("Error: Dataset file not found.")

except Exception as error:
    print("Error while loading dataset:", error)
```

This prevents the program from crashing due to common file or data-loading errors.

---

# 🖥️ Menu-Driven Interface

The project includes a menu-driven interface for easier interaction.

```text
==============================================
       PANDAS ANALYZER & DATA VISUALIZATION
==============================================
1. Load Dataset
2. Explore Data
3. Perform DataFrame Operations
4. Handle Missing Data
5. Generate Descriptive Statistics
6. Data Visualization
7. Save Visualization
8. Exit
==============================================
```

The user can select an option by entering the corresponding number.

---

# 🔍 Explore Data Menu

The Explore Data section provides:

```text
1. Display first 5 rows
2. Display last 5 rows
3. Display column names
4. Display data types
5. Display basic information
```

The project also provides descriptive information about the dataset.

---

# 🧹 Missing Data Menu

The Missing Data section provides:

```text
1. Display rows with missing values
2. Fill missing values with mean
3. Drop rows with missing values
4. Replace missing values with specific value
```

---

# 📊 Visualization Menu

The visualization section provides:

```text
1. Bar Chart
2. Line Chart
3. Scatter Plot
4. Pie Chart
5. Histogram
6. Stack Plot
```

Additional visualizations are implemented through the class methods, including:

- Heatmap
- Box Plot
- Subplots

---

# 📌 Sample Analysis Results

Based on the provided dataset:

| Metric | Result |
|--------|--------:|
| Total Sales | 583000 |
| Average Sales | 29150 |
| Total Profit | 91400 |
| Average Profit | 4570 |
| Number of Records | 20 |
| Best Performing Product | Laptop |
| Best Performing Region | North |

---

# 🏆 Product Sales Summary

| Product | Total Sales |
|---------|------------:|
| Laptop | 235000 |
| Mobile | 138000 |
| Tablet | 118000 |
| Headphones | 57000 |
| Keyboard | 35000 |

---

# 🌍 Regional Sales Summary

| Region | Total Sales |
|--------|------------:|
| North | 143000 |
| South | 142000 |
| West | 127500 |
| East | 124500 |

---

# ▶️ Example Usage

The analyzer object can be created using:

```python
analyzer = SalesDataAnalyzer()
```

The dataset can then be loaded using:

```python
analyzer.load_data("sales_data.csv")
```

Data exploration:

```python
analyzer.explore_data()
```

Statistical analysis:

```python
analyzer.statistical_analysis()
```

Visualization:

```python
analyzer.visualize_data("bar")
```

Save visualization:

```python
analyzer.save_visualization(
    "sales_visualization.png"
)
```

Run the complete menu-driven system:

```python
main_menu(analyzer)
```

---

# 🚀 How to Run

## Option 1: Google Colab

1. Open Google Colab.
2. Upload `Pandas_Analyzer.ipynb`.
3. Upload `sales_data.csv`.
4. Run the notebook cells in order.
5. Execute:

```python
main_menu(analyzer)
```

6. Use the menu to perform analysis and visualization.

---

## Option 2: Jupyter Notebook

Install the required libraries:

```bash
pip install pandas matplotlib seaborn
```

Then open:

```text
Pandas_Analyzer.ipynb
```

Run the notebook cells in sequence.

---

# 📦 Requirements

The project requires:

```text
Python 3.x
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook / Google Colab
```

Install the main libraries using:

```bash
pip install pandas matplotlib seaborn
```

NumPy is also used by the project and is commonly available in Jupyter/Colab environments.

---

# 🔁 Project Execution Flow

```text
Start
  │
  ▼
Create SalesDataAnalyzer Object
  │
  ▼
Load sales_data.csv
  │
  ▼
Explore Dataset
  │
  ▼
Clean Missing Data
  │
  ▼
Perform NumPy Operations
  │
  ▼
Perform Mathematical Operations
  │
  ▼
Combine / Split Data
  │
  ▼
Search / Sort / Filter
  │
  ▼
Aggregate Functions
  │
  ▼
Statistical Analysis
  │
  ▼
GroupBy / Transform
  │
  ▼
Pivot Table
  │
  ▼
Re-index Data
  │
  ▼
Create Visualizations
  │
  ▼
Save Visualization
  │
  ▼
Export Analysis Results
  │
  ▼
Display Conclusion
  │
  ▼
Exit
```

---

# 🧠 Concepts Demonstrated

This project demonstrates the following concepts:

### Python

- Classes
- Objects
- Methods
- Constructors
- Destructors
- Exception Handling
- Functions
- Conditional Statements
- Loops

### Pandas

- DataFrame
- CSV reading
- Data cleaning
- Missing values
- Data type conversion
- GroupBy
- Transform
- Pivot Table
- Sorting
- Filtering
- Aggregation
- Concatenation
- Re-indexing
- Statistical functions

### NumPy

- Array conversion
- Indexing
- Slicing
- Numerical operations

### Matplotlib

- Bar Chart
- Line Chart
- Scatter Plot
- Pie Chart
- Histogram
- Stack Plot
- Subplots
- Figure saving

### Seaborn

- Heatmap
- Box Plot
- Styling

---

# 🎓 Key Learning Outcomes

After completing this project, the following practical skills are demonstrated:

- Working with real-world style tabular data
- Understanding Pandas DataFrames
- Performing data cleaning
- Handling missing values
- Performing numerical calculations
- Using NumPy with Pandas
- Performing statistical analysis
- Grouping and aggregating data
- Creating pivot tables
- Searching and filtering datasets
- Creating meaningful visualizations
- Using Object-Oriented Programming
- Creating menu-driven Python applications
- Saving analysis outputs
- Documenting a complete data analysis project

---

# 📝 Assumptions

The following assumptions were made for this project:

1. The dataset is synthetic and created for academic demonstration.
2. Sales and Profit columns contain numerical values.
3. Year is stored as a numerical column.
4. Date values are converted to Pandas datetime format.
5. Missing numerical values are handled using column mean where applicable.
6. Region and Product are treated as categorical fields.
7. The analysis focuses on sales and profit-related information.
8. Visualizations are created from the available dataset.

---

# ⭐ Project Highlights

| Feature | Status |
|---------|--------|
| Pandas DataFrame | ✅ |
| NumPy Operations | ✅ |
| Data Cleaning | ✅ |
| Missing Value Handling | ✅ |
| Mathematical Operations | ✅ |
| DataFrame Combining | ✅ |
| DataFrame Splitting | ✅ |
| Search / Sort / Filter | ✅ |
| Aggregation | ✅ |
| Statistical Analysis | ✅ |
| Pivot Table | ✅ |
| GroupBy / Transform | ✅ |
| Re-indexing | ✅ |
| Matplotlib Charts | ✅ |
| Seaborn Charts | ✅ |
| Subplots | ✅ |
| Visualization Saving | ✅ |
| CSV Export | ✅ |
| OOP Implementation | ✅ |
| Exception Handling | ✅ |
| Menu-Driven Interface | ✅ |

---

# 🏁 Conclusion

The **Pandas Analyzer & Data Visualization** project successfully demonstrates how Python libraries can be used to perform complete sales data analysis.

The project combines:

```text
Python
   +
Pandas
   +
NumPy
   +
Matplotlib
   +
Seaborn
   +
OOP
   +
Data Visualization
```

The dataset was successfully loaded, explored, cleaned, analyzed and visualized.

Important insights such as total sales, average sales, total profit, product performance and regional performance were calculated.

The project also demonstrates practical DataFrame operations, statistical analysis, visualization techniques, menu-driven programming and Object-Oriented Programming.

Overall, this project provides a practical foundation for understanding **Data Analysis and Data Visualization using Python**.

---

# 👨‍💻 Developer

### Chand Khimani

**BCA — Final Year**  
**Data Analysis Course**

**Guided By:** Girish Gondaliya Sir

---

<div align="center">

### 🚀 Keep Learning. Keep Building. Keep Growing.

**Happy Coding! 💻📊**

Thank you for checking out this project! ❤️

</div>
