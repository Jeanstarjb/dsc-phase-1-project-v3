### Aviation Risk Analysis: A Data-Driven Approach to Aircraft Acquisition
###Project Overview
This project analyzes historical aviation accident data from the National Transportation Safety Board (NTSB) to provide data-driven recommendations for a company looking to enter the aviation industry. The primary goal is to identify aircraft with the lowest risk profile to guide the initial fleet acquisition strategy. By exploring trends in accident frequency, severity, and contributing factors, this analysis translates raw data into actionable business intelligence.

####Business Problem
A corporation is planning to diversify its portfolio by creating a new aviation division to purchase and operate commercial and private aircraft. As the company has no prior experience in this sector, it requires a thorough risk assessment of potential aircraft to make informed, low-risk purchasing decisions. This project serves as that initial analysis.

####Data Source
The analysis is based on the NTSB's aviation accident dataset, which contains records from 1982 to 2022. This rich dataset provides detailed information on civil aviation accidents in the United States, including aircraft make and model, engine type, damage severity, location, weather conditions, and injury counts.

####Methodology
The project follows a structured data analysis process:

####Data Cleaning & Preparation:

Standardized column names and data formats (e.g., converting dates, standardizing text to uppercase).

Dropped irrelevant columns with high percentages of missing data or low relevance to the business problem.

Handled missing values in key columns through logical imputation (e.g., filling missing injury counts with 0) or filling with "Unknown" to retain records.

Filtered the dataset to focus on incidents within the United States for consistency.

####Exploratory Data Analysis (EDA):

Performed univariate and bivariate analysis to understand the relationships between different variables.

Created visualizations (bar charts, count plots) to identify patterns related to:

Aircraft Manufacturers

Number of Engines

Aircraft Build Type (Commercial vs. Amateur)

Geographical Location and Weather

Incident Outcomes (Fatal, Injured, Uninjured)

####Conclusion & Recommendations:

Synthesized the findings from the EDA to derive insights.

Formulated three concrete, data-driven recommendations to guide the company's business strategy.

####Key Findings & Visualizations
Popularity vs. Risk: While manufacturers like Cessna and Piper have the highest number of total incidents, this is a function of their market dominance, not necessarily an indicator of poor safety. A rate-based analysis (e.g., accidents per flight hour) is needed for a true comparison.

Engine Redundancy is Key: Multi-engine aircraft have a significantly better safety profile than single-engine aircraft, with far fewer fatal and non-fatal incidents.

Certified Aircraft are Safer: Commercially manufactured aircraft, which undergo rigorous FAA certification, are demonstrably safer than amateur-built or "experimental" aircraft.

Environmental Factors Matter: Accidents are concentrated in high-traffic areas (e.g., Miami, Houston) and regions with challenging weather/terrain (e.g., Anchorage, AK).

####Final Recommendations
Prioritize Multi-Engine, Commercially-Built Aircraft: To minimize operational risk and liability, the initial fleet should consist exclusively of commercially manufactured, multi-engine planes.

Focus on Established Manufacturers: Acquire aircraft from popular brands like Cessna and Piper. Their market prevalence ensures a robust support network for maintenance, parts, and qualified pilots.

Adopt a Rate-Based Risk Assessment Model: When evaluating specific aircraft models, the company must use normalized metrics like "fatalities per incident" and "percentage of uninjured occupants" rather than relying on misleading raw incident counts.

####Repository Contents
Aviation_Risk_Analysis.ipynb: The main Jupyter Notebook containing all data cleaning, analysis, and visualization code.

presentation.pdf: A non-technical slide deck summarizing the project's findings and recommendations for business stakeholders.

/data: Folder containing the raw AviationData.csv file.

README.md: This file.

How to Run This Project
Clone the repository to your local machine.

Ensure you have the following Python libraries installed:

pandas

numpy

matplotlib

seaborn

Open and run the Aviation_Risk_Analysis.ipynb notebook in a Jupyter environment.

Author
Jeff Mogaka


