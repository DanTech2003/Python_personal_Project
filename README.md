# Python_personal_Project
## Project Overview
This project involves a comprehensive exploratory data analysis (EDA) and data cleaning of a music records dataset containing over 10,000 entries. The goal was to refine the dataset by handling missing values and erroneous entries (such as invalid years, tempo, and loudness) to produce accurate visualizations of musical trends from 1920 to 2010.
## Tools Used
-- Python
-- Pandas
-- seaborn
-- Numpy
-- Matplotlib
-- Jupyter Notebook

## project Task
-- Import Excel dataset
-- Data Cleaning 
-- Exploratory Data Analysis
-- Visualization

## Song Data Analysis & Cleaning Project
-- Tech Stack
-- Language: Python
-- Libraries: Pandas, NumPy, Matplotlib
-- Environment: Jupyter Notebook
## Data Cleaning Process
A significant portion of this project focused on data integrity. Key cleaning steps included:
Handling Nulls: Identified missing values in the title column and filled them with "Unknown" to maintain dataset size.
Correcting Erroneous Years: Discovered 5,309 records with a year_released of 0. These were isolated to prevent skewing chronological trends.
Validating Physics of Sound: * Filtered out songs with a tempo \le 0 (28 records found).
Addressed loudness values \ge 0, as Decibels (dB) in digital audio are typically measured in negative values (0dB being the maximum ceiling).
## Key Insights & Visualizations
1. Loudness Trends Over Time
By creating a pivot table of the mean loudness per year, I generated a line graph showing the evolution of song dynamics.
Observation: There is a visible upward trend in average loudness (becoming "less negative") starting around the 1990s, likely reflecting the "Loudness War" in the music industry.
2. Distribution of Songs per Year
I analyzed the volume of records across the century to understand the dataset's density.
Observation: The dataset shows exponential growth in song records reaching its peak in the mid-2000s, providing a robust sample size for modern music analysis


## Global Electricity Production Analysis (2022–2024)
## Project Overview
This project analyzes global electricity production trends by source and location. The data was scraped from Wikipedia, cleaned using Python, and analyzed to compare the growth of renewable vs. fossil fuel energy sources.
## Key Insights
-- Dominant Sources: Coal remains the leading source of global energy production, followed by Gas and Hydro.
-- The Energy Gap: While Fossil Fuel production is significantly higher in total TWh, Renewable Energy is showing a clear upward trajectory.
-- Top Producers: Major economies like China and the United States lead in total production, with China showing significant output across multiple sources.
-- Sustainability: Low-carbon sources (Nuclear + Renewables) are growing, but Fossil Fuels (Coal, Gas, Oil) still account for the majority of the global energy mix.
**Technical Stack**
-- Language: Python
-- Libraries: * Pandas: Data manipulation and cleaning.
-- NumPy: Numerical operations.
-- Requests: Web scraping/fetching HTML content.
-- Matplotlib: Data visualization and trend plotting.
-- Environment: JupyterLab
## Data Acquisition & Cleaning
Data was extracted from a Wikipedia list of countries by electricity production.
Web Scraping: Used requests with custom headers to fetch the table and pd.read_html for parsing.
Data Cleaning: * Handled multi-level column indexing using droplevel().
Renamed complex headers for better readability.
Converted data types (e.g., converting 'Year' and 'Nuclear' to integers).
Reordered columns for a more logical "Year-First" flow.
## Exploratory Data Analysis (EDA)
Grouped data by Year to find peak production periods.
Analyzed the safest environment options by comparing broad energy categories.
Identified the lowest contributing energy source globally (Geothermal).
## Visualizations
Renewable vs. Fossil Energy Production Over Time
The line chart demonstrates the growth of energy production from 2022 to 2024. While both sectors are growing to meet global demand, the gap between Fossil Fuels and Renewables remains a key area for climate policy focus.
Overall Energy Mix by Source
A horizontal bar chart ranking energy sources by total production (TWh). This highlights the heavy reliance on Coal and Gas, and the emerging role of Wind and Solar in the global mix.

## Key Analytical Insights
The 40% Threshold: 2024 marked the first time in modern history that low-carbon sources (Nuclear & Renewables) provided over 40% of global power.  
Solar as a Growth Engine: Solar energy is now the primary driver of global grid expansion, meeting nearly half of all new electricity demand.
Safety-Climate Correlation: My analysis confirms a direct link between environmental safety and carbon intensity; low-carbon sources like Wind and Solar are not just cleaner, but significantly safer for human populations.
Regional Divergence: While the West is seeing a decline in coal, global totals remain high due to rapid industrialization in the BRICS nations, specifically China and India.

## Third Project Overview
This project involves a comprehensive End-to-End Data Pipeline that bridges PostgreSQL and Python to analyze a massive airline dataset (98,000+ records). I engineered a secure database connection, performed extensive data cleaning in Pandas, and developed a suite of visualizations to uncover passenger behavior and operational trends.
##  Key Insights & Findings
-- Demographic Dominance: The 60+ age group represents the largest passenger segment, while the 18-30 demographic is the smallest. Gender distribution is remarkably balanced (49.6% Male / 49% Female).
-- Global Hubs: North America (NAM) accounts for 32.5% of all flights, followed by Asia. China and Indonesia are the top two passenger nationalities.
-- Operational Bottleneck: There is a near-equal split (~33% each) between On Time, Delayed, and Cancelled flights. This high cancellation/delay rate suggests significant room for operational optimization.
-- Seasonal Stability: Flight volume and cancellations remain relatively consistent across seasons, with a slight peak in activity during Summer.
-- Top Route: The most frequent flight path identified is Böblingen Flugfeld → PHM.
## Technical Highlights
-- Database Integration: Used SQLAlchemy and psycopg2 for seamless SQL-to-DataFrame extraction.
-- Security: Implemented getpass to handle database credentials securely.
-- Data Engineering: Created custom Season mapping and Age Group binning to enhance analytical depth.
-- Visualization: Leveraged Seaborn and Matplotlib for categorical, distribution, and trend analysis.

## Author
Daniel Oluwasegun Ogunfadewo Business and Development Analysts
specializing in SQL, Python and PowerBI to turn raw data into strategic business insights.

