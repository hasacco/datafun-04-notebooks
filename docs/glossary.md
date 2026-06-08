# Glossary

This Module 4 glossary defines common terms used in notebooks,
exploratory data analysis (EDA), pandas, and related Python tools.

## Section 1. Notebook Basics

### Notebook

A notebook is an interactive document that combines
code, output, text, tables, charts, and notes in one file.
In data work, notebooks are often used for exploration,
documentation, and early analysis.

### Jupyter Notebook

A Jupyter Notebook is a common notebook format used for Python,
data analysis, visualization, and scientific computing.
Jupyter notebooks usually have the file extension `.ipynb`.

### Markdown Cell

A Markdown cell contains formatted text, not Python code.
Use Markdown cells to write headings, explanations,
instructions, observations, and conclusions.

### Code Cell

A code cell contains Python code that can be run.
When a code cell runs, it may produce printed text,tables, charts, logs, or other output.

### Cell Output

Cell output is the result shown after running a code cell.
Output may include text, tables, error messages, charts, or images.

### Run a Cell

To **run a cell** means to execute the code or render the Markdown in that cell.
Running a Python cell sends its code to the active Python environment.

### Run All

**Run All** means running every cell in the notebook from top to bottom.
Notebooks can become inconsistent if cells are run out of order.

### Kernel

The **kernel** is the running Python process connected to the notebook.
The kernel remembers variables, imports, functions, and
objects created while the notebook is running.

### Restart Kernel

**Restarting** the kernel clears the notebook's active memory.
This is useful when checking whether a notebook runs correctly from a clean start.

### Python Environment

A Python environment is the set of Python packages and tools available to a project.
Our project environment comes from the `.venv` folder created by `uv`.

### Notebook State

Notebook state refers to the current memory of the running notebook kernel.
A notebook may appear to work because of old variables still stored in memory.
Restarting the kernel and running all cells helps detect this problem.

### Reproducible Notebook

A reproducible notebook can be run from top to bottom and produce the expected results.
A notebook is more reproducible when imports, configuration,
data loading, cleaning, analysis, and visualizations appear in order.

## Section 2. Exploratory Data Analysis

### Exploratory Data Analysis

Exploratory Data Analysis, or EDA, is the process of examining a dataset
to understand its structure, quality, patterns, and limitations.
EDA usually happens before formal modeling or final reporting.

### Dataset

A dataset is a collection of data used for analysis.
A dataset may come from a CSV file, database, API, spreadsheet, package, or built-in library source.

### Observation

An observation is one recorded item in a dataset.
In a table, each row usually represents one observation.

### Variable

A variable is a measured or recorded **feature**.
In a table, each column usually represents one variable.

### Row

A row is a horizontal record in a table.
Each row usually represents one observation.

### Column

A column is a vertical field in a table.
Each column usually represents one variable.

### Tabular Data

Tabular data is data arranged in rows and columns.
Spreadsheets, CSV files, and database tables are common forms of tabular data.
Python often uses the **pandas** (panel data set) package to work with tabular data.

### Data Dictionary

A data dictionary describes the **columns** in a dataset.
It often includes column names, data types, meanings, valid values, units, and missing-value information.

### Data Quality

Data quality refers to how suitable the data is for analysis.
Common data quality issues include missing values, duplicates,
inconsistent categories, invalid values, and incorrect data types.

### Missing Value (NaN)

A missing value is a value that is absent, unknown, or not recorded.
In pandas, missing values often appear as `NaN` for **not a number**.

### Duplicate Row

A **duplicate row** is a row that appears more than once in a dataset.
Duplicates may be valid, accidental, or evidence of a data collection problem.

### Outlier

An **outlier** is a value that is unusually far from most other values.
Outliers may be errors, rare events, or important signals.

### Distribution

A **distribution** describes how values are spread across a variable.
For numeric data, a distribution may show center, spread, skew, and unusual values.

### Summary Statistics

**Summary statistics** are numeric summaries of a variable.
Common examples include count, mean, median, standard deviation,
minimum, maximum, and quartiles.

### Descriptive Statistics

**Descriptive statistics** is a general term for metrics
that summarize what is present in a dataset.
They describe the dataset but do not, by themselves,
prove causes or make predictions.

### Count

Count is the number of values or observations.
In pandas, count often excludes missing values.

### Mean

The mean is the arithmetic average.
It is calculated by adding values and dividing by the number of values.

### Median

The median is the middle value after values are sorted.
The median is often less affected by outliers than the mean.

### Standard Deviation

Standard deviation measures how spread out numeric values are around the mean.
A larger standard deviation means values vary more.

### Minimum

The minimum is the smallest value in a variable.

### Maximum

The maximum is the largest value in a variable.

### Range

The range is the difference between the maximum and minimum values.

### Quartile

A **quartile** divides sorted numeric data into **four parts**.
The 25th percentile, median, and 75th percentile are common quartiles.

### Correlation

**Correlation** measures the strength and direction of a linear relationship between two numeric variables.
Correlation does not prove causation.

### Correlation Matrix

A **correlation matrix** is a table showing correlations among multiple numeric variables.
The diagonal values are always 1.0 because each variable is perfectly correlated with itself.

### Grouping

Grouping means splitting data into categories before calculating summaries.
For example, penguin measurements might be grouped by species.

### Aggregation

Aggregation means calculating summary values for groups of data.
Common aggregations include count, mean, minimum, maximum, and standard deviation.

### Cleaned Data

Cleaned data is data that has been adjusted or filtered to support analysis.
Cleaning may include removing missing values, correcting types,
renaming columns, or selecting relevant rows.

### Clean View

A clean view is a modified version of the data used for analysis
while preserving the original dataset.
A clean view helps avoid accidentally changing the raw data.

## Section 3. Python Basics for Notebooks

### Python

Python is the programming language used in the notebook.
It is widely used for data analysis, automation, visualization,
machine learning, and scientific computing.

### Import

An import brings external code into the current Python session.
For example, `import pandas as pd` makes the pandas library available using the name `pd`.

### Library

A library is a collection of reusable code.
Examples used in EDA include pandas, NumPy, Matplotlib, and Seaborn.

### Package

A package is an installable collection of Python modules.
Packages are usually installed into a Python environment.

### Module

A module is a Python file or package component that contains code.
Modules may contain functions, classes, constants, and other definitions.

### Local Variable

A local variable is a name you choose that refers to a value or object.
For example, `df` often refers to a pandas DataFrame.

### Object

An object is a value with data and behavior.
In pandas, a DataFrame is an object with rows, columns, methods, and attributes.

### Function

A function is reusable code that performs a task.
For example, `print()` displays text, and `len()` returns the length of something.

### Method

A method is a function attached to an object.
For example, `df.head()` calls the `head()` method on the DataFrame named `df`.

### Attribute

An attribute is a value stored on an object.
For example, `df.shape` is an attribute that gives the number of rows and columns.

### Argument

An argument is a value passed into a function or method.
For example, in `df.head(10)`, the value `10` is an argument.

### Keyword Argument

A keyword argument is an argument passed by name.
For example, in `df.dropna(subset=cols_required)`, `subset` is a keyword argument.

### List

A list is an ordered collection of values.
For example, a list of column names may look like `["bill_length_mm", "body_mass_g"]`.

### Tuple

A tuple is an ordered collection of values that is usually treated as fixed.
For example, `df.shape` returns a tuple like `(344, 7)`.

### String

A string is text data.
Column names, labels, file paths, and category names are often strings.

### Integer

An integer is a whole number.
Row counts and column counts are usually integers.

### Float

A float is a number with a decimal point.
Measurements such as body mass or bill length may be stored as floats.

### Boolean

A Boolean is a true-or-false value.
Boolean values are often used for filtering data.

## Section 4. Using the pandas Library

### pandas library (critical for analysts)

pandas is a Python library for working with structured data.
It is especially useful for tabular data with rows and columns.

### DataFrame

A DataFrame is a two-dimensional pandas table.
It has rows, columns, column names, and an index.

### df

`df` is a common variable name for a DataFrame.

### Series

A Series is a one-dimensional pandas object.
A single DataFrame column is usually a Series.

### Index

The index labels the rows of a DataFrame or Series.
The default index is often a sequence of numbers starting at 0.

### Column Name

A column name is the label for a column in a DataFrame.
Column names are used to select, filter, group, and summarize data.

### dtype

`dtype` means data type.
In pandas, each column has a dtype such as `int64`, `float64`, `object`, `string`, or `category`.

### shape

`shape` is a DataFrame attribute that returns the number of rows and columns.
For example, `(344, 7)` means 344 rows and 7 columns.

### head()

`head()` shows the first few rows of a DataFrame.
It is often used at the beginning of EDA to preview the data.

### tail()

`tail()` shows the last few rows of a DataFrame.
It can help confirm how the dataset ends.

### info()

`info()` prints column names, data types, non-null counts, and memory usage.
It is useful for checking structure and missing values.

### describe()

`describe()` calculates summary statistics for numeric columns by default.
It commonly returns count, mean, standard deviation, minimum, quartiles, and maximum.

### isna()

`isna()` checks whether values are missing.
It returns true for missing values and false for present values.

### isnull()

`isnull()` is another pandas method for checking missing values.
In pandas, `isnull()` and `isna()` are commonly used for the same purpose.

### notna()

`notna()` checks whether values are present.
It returns true for non-missing values.

### sum()

`sum()` adds values.
When used with Boolean true-or-false values, true values are counted as 1 and false values as 0.

### mean()

`mean()` calculates the arithmetic average.
When used on Boolean values, it can calculate the proportion of true values.

### duplicated()

`duplicated()` identifies duplicate rows.
It returns true for rows that repeat earlier rows.

### dropna()

`dropna()` removes rows or columns with missing values.
Using `subset=` limits the missing-value check to selected columns.

### copy()

`copy()` creates a separate copy of a DataFrame or Series.
It is often used to avoid accidentally modifying the original data.

### select_dtypes()

`select_dtypes()` selects columns by data type.
For example, it can select only numeric columns.

### groupby()

`groupby()` splits data into groups based on one or more columns.
It is commonly followed by an aggregation method.

### agg()

`agg()` applies one or more aggregation functions to grouped data.
For example, it can compute count, mean, standard deviation, minimum, and maximum by group.

### corr()

`corr()` calculates correlations among numeric columns.
It is commonly used to create a correlation matrix.

### value_counts()

`value_counts()` counts how often each unique value appears.
It is useful for categorical columns.

### sort_values()

`sort_values()` sorts a DataFrame or Series by values.
It can sort in ascending or descending order.

### subset

A subset is a selected part of a larger dataset.
A subset may include selected rows, selected columns, or both.

### Filter

A filter selects rows that meet a condition.
For example, a filter might keep only rows where species is Gentoo.

### Chaining

Chaining means calling multiple methods in sequence.
For example, `df.isna().sum().sort_values()` chains several operations.

## Section 5. Visualization Terms

### Visualization

A visualization is a graphical representation of data.
Charts help reveal patterns, comparisons, distributions, and relationships.

### Chart

A chart is a visual display of data.
Common chart types include bar charts, histograms, scatter plots, box plots, and heatmaps.

### Figure

A figure is the full Matplotlib drawing area.
A figure may contain one or more plots.

### Axes

Axes are the plot area where data is drawn.
In Matplotlib and Seaborn, an Axes object is often used to set titles, labels, and formatting.

### Bar Chart

A bar chart compares values across categories.
It is useful for counts, averages, or totals by group.

### Histogram

A histogram shows the distribution of a numeric variable.
It groups values into bins and shows how many observations fall into each bin.

### Scatter Plot

A scatter plot shows the relationship between two numeric variables.
Each point represents one observation.

### Box Plot

A box plot summarizes the distribution of a numeric variable.
It shows the median, quartiles, spread, and possible outliers.

### Heatmap

A heatmap uses color intensity to represent values in a table.
Correlation matrices are often visualized as heatmaps.

### x-axis

The x-axis is the horizontal axis of a chart.
It often shows categories or an independent numeric variable.

### y-axis

The y-axis is the vertical axis of a chart.
It often shows counts, measurements, or a dependent numeric variable.

### Label

A label describes an axis, category, point, or legend item.
Good labels make charts easier to understand.

### Title

A title explains what a chart shows.
A good chart title should be specific enough to stand alone.

### Legend

A legend explains visual encodings such as color, marker style, or group.
For example, species may be shown using different colors.

### Color Encoding

Color encoding uses color to represent categories or values.
In EDA, color is often used to distinguish groups.

## Section 6. Python Libraries Used

- **NumPy** is a Python library for numeric computing.
  It provides arrays and mathematical functions used by many data science libraries.
- **pandas** is used for reading, cleaning, transforming, summarizing, and analyzing structured data.
  Its primary data structures are DataFrame and Series.
- **Matplotlib** is a Python visualization library.
  It provides detailed control over figures, axes, labels, titles, and chart layout.
- **Seaborn** is a statistical visualization library built on top of Matplotlib.
  It provides convenient functions for charts such as scatter plots, histograms, box plots, and heatmaps.
- **datafun_toolkit** is a course-support package used for shared utilities such as logging.
  It provides functions such as `get_logger()` and `log_header()`.

## Section 7. Logging and Output

### Logger

A logger records messages from code.
In notebooks, a logger can show progress, data checks, warnings, and debugging details.

### Log Message

A log message is a recorded message from the program.
Examples include "Loading dataset" or "Duplicate rows detected: 0".

### Log Level

A log level indicates the importance or purpose of a message.
Common levels include DEBUG, INFO, WARNING, ERROR, and CRITICAL.

- DEBUG messages provide detailed information for troubleshooting.
  They are useful during development but may be too detailed for final reports.

- INFO messages describe normal progress.
  They are useful for showing what the notebook is doing.

- WARNING messages indicate something unexpected or potentially problematic.
  A warning does not always mean the notebook must stop.

- ERROR messages indicate that something failed.
  An error may stop a cell from completing.

### print()

`print()` displays text output.
It is simple and useful, but less structured than logging.

### display()

`display()` renders rich output in a notebook.
It is useful for showing DataFrames as formatted tables.

## Section 8. Professional Communication

### Standard Header

A standard header gives the notebook title, author, repository, purpose, date, and dataset information.
It helps readers understand what the notebook is and where it belongs.

### Purpose

The purpose explains why the notebook exists.
A clear purpose helps readers understand what the notebook is meant to demonstrate or investigate.
The ability to understand and covey your purpose for the exploration is critical.

### Repository Link

A repository link points to the project source.
It helps readers find related files, instructions, and version history.

### Dataset Source

The dataset source explains where the data came from.
This is important for credibility, reproducibility, and citation.
The ability to document a datasource is critical.

A **citation** gives credit to the data creators or source.
Datasets should be cited when the source provides citation information.

### Clean vs Stale Output

Clean output means the notebook output is relevant, readable, and
not cluttered with stale or unnecessary results.
Before sharing a notebook, verify everything appears correctly when
displayed in your GitHub repository.

Stale output is output that no longer matches the current code.
This can happen when code is edited after cells have already been run.

### Save Notebook

Saving a notebook writes the current code, Markdown, and possibly outputs to the `.ipynb` file.
Always save after important changes.

### Commit

A commit records a saved version of files in Git.
A good commit captures a meaningful checkpoint in the project.

## Section 9. Common EDA Workflow Terms

### Load

Loading means bringing data into the notebook.
For example, a dataset may be loaded into a pandas DataFrame.

### Inspect

Inspecting means looking at the structure and contents of the data.
Common inspection methods include `head()`, `info()`, `shape`, and `columns`.

### Clean

Cleaning means preparing data for analysis.
This may include handling missing values, fixing types, renaming columns, or removing duplicates.

### Transform

Transforming means changing data into a more useful form.
Examples include creating new columns, filtering rows, or grouping data.

### Visualize

Visualizing means creating charts from data.
Charts help identify patterns that may not be obvious from tables alone.

### Interpret

Interpreting means explaining what the analysis suggests.
Interpretation should stay grounded in the evidence shown by the data.

### Finding

A finding is an observation supported by the analysis.
Findings should be specific and connected to evidence from tables, statistics, or charts.

### Summarize

Summarizing means reducing data into useful statistics or tables.
Examples include counts, means, grouped summaries, and correlation matrices.

### Limitation

A limitation is something the data or analysis cannot fully answer.
Good EDA notes limitations clearly instead of overstating conclusions.

### Next Steps

A next step is a reasonable action after EDA.
Examples include additional cleaning, collecting more data, modeling,
or investigating a pattern more closely.
