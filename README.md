## Aircraft Safety Performance Metrics
This project focuses on analyzing aviation accident data to develop insights and metrics related to aircraft safety performance. The goal is to identify factors that influence the safety of the aircraft make and model, operational costs, financial impact and the marketability of the aircraft based on safety performance.

### Table of Contents
- [Data](#data)
- [Analysis Overview](#analysis-overview)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

### Data
The Aviation dataset in this analysis includes aviation accident data that provides information about aircraft make and model, total number of injuries, weather conditions, and accident circumstances. Key columns in the dataset include:
- **Aircraft Make:** The manufacturer and model of the aircraft.
- **Injury Severity:** The severity of injuries caused by the accident (e.g., fatal, serious, or minor).
- **Accident Location:** The country and city where the accident occurred.
- **Aircraft Damage:** The level of damage sustained by the aircraft during the accident.
- **Purpose of flight:** The reason as to why the passenger swere flying.

## Analysis Overview
The primary goal of this analysis is to uncover key insights from aviation accident data that can contribute to improving safety, optimizing operational costs,minimizing financial expenditure and enhancing the marketability of aircraft. The analysis is structured around the following objectives:
- **Safety:** Understanding factors such as  weather conditions, number of engines  and engine type  that influence the severity of injuries during accidents to inform safety protocols and mitigation strategies.
- **Operational Costs:** Identifying patterns like number of engines, amatuer built and aircraft damage in accident data to minimize costs associated with operational disruptions and repairs.
- **Financial Impact:** Assessing the relationship between the severity of accidents and their associated financial consequences, including aircraft damage, aircraft make and the purpose of the flight.
- **Marketability:** Evaluating how safety records and performance metrics influence the attractiveness of aircraft in the market, which could impact the number of flights people take per country and operational costs.

### Key Steps in the Analysis:
### **1. Data Structure Overview:**
- **Objective:** Understand the dataset’s variables, dimensions, and overall structure.
- **Action:** 
  - I first examined the dataset to check the number of rows and columns.
  -  I Identified the types of variables (e.g., categorical, continuous) and their data types.

### **2. Data Cleaning:**
- **Objective:** Prepare the dataset for analysis by addressing data quality issues  and missing data.
- **Action:** 
  - Handled **missing values** through imputation by adding mean to numerical columns and mode for categorical columns.
  - **Removed irrelevant columns** that didn’t contribute to the analysis objectives.

### **3. Descriptive Statistics:**
- **Objective:** Summarize the main characteristics of the dataset.
- **Action:**
  - Calculated **summary statistics** (mean, median, mode, standard deviation, min, and max) for continuous variables.
  - Calculated **count statistics** for the categorical values.
  - Calculated  the range between the maximum and mminmum for categorical columns
    
### **4. Feature Engineering:**
- **Objective:** Enhance the dataset by creating new variables and refining existing ones for better insights.
- **Action:**
  - Created new variables based on existing ones, such as aggregating the total number of injuries and grouping them by has hghest injury count
  - Removed any variables that were redundant or not useful for the analysis objectives.

### **5. Exploratory Data Analysis (EDA):**
- **Objective:** Visually and statistically analyze the data to uncover trends, patterns, and insights.
- **Action:** 
  - **Univariate Analysis:** 
    - I began by exploring individual variables using  **visualizations** like **histograms** for continuous variables and **bar charts** for categorical variables.
  - **Bivariate Analysis:** 
    - I examined the relationships between two variables, using **scatter plots** for continuous variables and **box plots** for comparing continuous variables across categories. 
    - I also calculated **correlations** between key continuous variables (e.g., `total_injuries` and `accident_cost`) to identify linear relationships.
  - **Multivariate Analysis:** 
    - I extended the analysis to multiple variables simultaneously, using **pair plots** to visualize the relationships between several continuous variables.
    - **Heatmaps** were used to display the correlation matrix between multiple variables to detect clusters of related features.
    - I also grouped the data by categorical variables (e.g., `aircraft_make`, `flight_phase`) to compare how key metrics like `total_injuries` and `accident_cost` varied across these categories.

 




