Netflix Data Analysis (Python, NumPy, Pandas, Seaborn)

This case study explores the Netflix Titles dataset using Python programming, NumPy, Pandas, functional programming concepts, and data visualization.
The goal is to practice data manipulation, filtering, aggregation, and plotting using real-world data.

📁 Dataset

Netflix Titles Dataset
File used: netflix_titles.csv

Contains information about:

Title, Type (Movie / TV Show)

Director, Cast

Country

Date Added

Release Year

Rating, Duration

Genre (listed_in)

Description

🛠️ Tools & Libraries Used

Python

Pandas

NumPy

Matplotlib

Seaborn

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

📌 Questions & Solutions Overview
Q1. Movie titles longer than 10 characters (List Comprehension)

Used list comprehension to filter Movie titles based on length.

Q2. Titles starting with letter “S” (case-insensitive)

Used string methods with .str.lower() and .startswith().

Q3. NumPy statistics on release_year

Converted column to NumPy array.

Calculated mean, median, standard deviation.

Q4. Count shows released before 2000

Used a for loop to count older releases.

Q5. Create title_length column

Used .map() with a lambda function.

Q6. Replace missing director names for Movies

Filled missing values only for Movies with "Not Available".

Q7. Shows added after 2018 using filter()

Converted date_added to datetime.

Used filter() and lambda.

Q8. NumPy array manipulation

Generated 5×3 random array.

Replaced even numbers with half their value.

Q9. Drama & Crime content filtering

Used .str.contains() on listed_in.

Q10. Extract year from date_added (Lambda)

Created added_year column.

Q11. Function: Top countries by number of titles
def top_country(df, n):
    return df['country'].value_counts().head(n)

Q12. First 5 titles with word “love” in description

Case-insensitive search using .str.contains().

Q13. Replace NaN values with mean (NumPy)

Used np.nanmean() and np.where().

Q14. NumPy stacking

Combined sales and profit arrays into a 2D array.

Q15. Top 10 countries producing Netflix content (Seaborn)

Visualized using bar chart.

Q16. While loop – duration > 100 minutes

Printed random titles until condition met.

Q17. Movies vs TV Shows by release decade

Created release_decade column.

Grouped and counted content type.

Q18. Countries with more than 200 titles

Used value_counts() filtering.

Q19. Sum of release years using reduce()

Functional programming with functools.reduce().

Q20. Histogram – titles released per year

Used Matplotlib histogram for trend visualization.

📊 Key Skills Demonstrated

Data Cleaning & Feature Engineering

List Comprehension & Lambda Functions

Functional Programming (map, filter, reduce)

NumPy Array Operations

GroupBy & Aggregation

Data Visualization (Matplotlib & Seaborn)

🎯 Learning Outcomes

Hands-on experience with real-world datasets

Strong understanding of Pandas & NumPy

Ability to combine programming logic with data analysis

Practice with visualization techniques

Improved problem-solving and coding skills

👨‍💻 Author

Name: Faizan Bhat
Course: Python / Data Analytics
Skills: Python, Pandas, NumPy, Data Visualization
