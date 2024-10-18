Tech Layoffs Analysis (2020 – 2024)

Overview:

This project analyzes global tech layoffs reported since the onset of the COVID-19 pandemic. Economic challenges like slow consumer spending, high interest rates, and inflation have pushed tech giants, including Meta, to lay off large parts of their workforce. For example, Meta reduced its workforce by 13% (11,000 employees). The objective of this analysis is to uncover trends and insights from the layoffs dataset.

Data Source:

This dataset compiles layoff data reported on:
- Bloomberg
- TechCrunch
- San Francisco Business Times
- The New York Times
The dataset covers layoffs between March 11, 2020, and July 20, 2024. For further reference, see Layoffs.fyi.

Project Goals:
1. Data Cleaning:
- Handling Missing Values: Filtered out records with missing values in critical fields using WHERE clauses to ensure data integrity.
- Removing Duplicates: Applied SELECT DISTINCT to eliminate duplicate entries from the dataset.
- Standardizing Data Types: Ensured consistent data types across relevant fields by using CAST() or CONVERT() functions for numeric conversions, particularly in the percentage_laid_off field.

2. Exploratory Data Analysis (EDA):
- Aggregate Functions: Utilized functions like SUM(), MAX(), and MIN() to analyze total layoffs and identify the largest single layoffs across companies.
- Grouping Data: Employed GROUP BY to aggregate layoffs by company, industry, and location, facilitating deeper insights into trends.
- Window Functions: Used DENSE_RANK() to rank companies by total layoffs within specific years, enabling a year-on-year comparison of layoffs.
- String Manipulation: Leveraged SUBSTRING() to extract year-month from dates for time series analysis of layoffs over time.

Technologies Used:
- SQL: For data cleaning and querying.
- GitHub: For version control and collaboration.
  
Insights:
- Startups were the most vulnerable, with many laying off 100% of their staff, often ceasing operations entirely.
- Even large, well-funded companies like Quibi failed despite raising billions in funding.
- Economic conditions, including inflation and high interest rates, continue to disrupt the tech sector.
- Geographic trends showed layoffs clustering in certain regions, reflecting both local and global economic pressures.

Future Work:
- Visualize trends using Python libraries (e.g., Matplotlib, Seaborn).
- Build predictive models to anticipate future layoffs and economic impact.

