## Aircraft Safety Performance Metrics
This project focuses on analyzing aviation accident data to develop insights and metrics related to aircraft safety performance. The goal is to identify factors that influence the safety of the aircraft make and model, operational costs, financial impact and the marketability of the aircraft based on safety performance.

### Table of Contents
- [Data](#data)
- [Analysis Overview](#analysis-overview)
- [Visulizations](#visualizations)
- [Results](#results)
- [Recommendations](#recommendations)
- [License](#license)

### Data
The Aviation dataset in this analysis includes aviation accident data that provides information about aircraft make and model, total number of injuries, weather conditions and accident circumstances. Key columns in the dataset include:
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
- **Objective:**To understand the dataset’s variables, dimensions, and overall structure.
- **Action:** 
  - I first examined the dataset to check the number of rows and columns.
  -  I Identified the types of variables both categorical  and continuous and their data types.

### **2. Data Cleaning:**
- **Objective:preparing the dataset for analysis by addressing data quality issues and missing data.
- **Action:** 
  - Handled **missing values** through imputation by adding mean to numerical columns and mode for categorical columns.
  - **Removed irrelevant columns** that didn’t contribute to the analysis objectives.

### **3. Descriptive Statistics:**
- **Objective:** Summarizing the main characteristics of the dataset.
- **Action:**
  - Calculated **summary statistics** mean, median, mode, standard deviation, min, and max for continuous variables.
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
    - I also calculated **correlations** between key continuous variables like `total_injuries` and `accident_cost` to identify linear relationships.
  - **Multivariate Analysis:** 
    - I extended the analysis to multiple variables simultaneously using **pair plots** to visualize the relationships between several continuous variables.
    - **Heatmaps** were used to display the correlation matrix between multiple variables to detect clusters of related features.
    - I also grouped the data by categorical variables like `aircraft_make`, `flight_phase` to compare how key metrics like `total_injuries` and `accident_cost` varied across these categories.
      
### Visualizations
I started by cleaning the data to ensure it was structured and ready for analysis. Afterward, I imported the cleaned data into Tableau, where I created interactive visualizations to explore key insights. These visualizations highlight important trends and relationships, such as safety metrics, financial impacts, and market opportunities within the aviation industry.The visualizations are available here. You can explore them through this link: [https://public.tableau.com/app/profile/linet.patriciah/viz/aircraftmetricsworkbook/AIRCRAFTSAFETYMETRICS#1].

### Results
### **1. Safety Analysis**
#### **Weather Condition vs. Severity of Injury**
I examined how adverse weather conditions like VMC highly influenced the severity of injuries in incidents.  
  **Key Insights**:
  - Severe weather incidents like VMC result in a higher percentage of fatal and serious injuries compared to incidents in IMC then UMC because it had the least number of injuries.
 
#### **Number of Injuries vs. Number of engines**
 I explored whether incidents involving a high number of injuries have a stronger correlation with the number of engines that the aircraft had.  
  **Key Insights**:
  - Aircraft with less number of engines have a disproportionately higher share of total injuries.
  - Correlation coefficient between number of injuries and the number of engines of the aircraft is weak positive correlation (/r/=).

### **2. Operational Analysis**
#### **Total Injuries vs. Amateur-Built vs. Number of Engines**
I investigated if amateur-built aircraft and the number of engines correlates with higher injury rates.  
  **Key Insights**:
  - The aircraft with faulty amatuer during building are associated with more injuries than professionally built ones due to construction quality variances.
  - Single-engine aircraft incidents result in more injuries per accident compared to multi-engine aircraft, especially in amateur-built cases.
  - Findings could indicate the number of engines significantly reduces injury risk.

### **3. Financial Analysis**
#### **Aircraft Make, Damage Level, and Total Injuries**
- I assessed how specific aircraft make and damage levels correlate with financial losses and injury rates.  
  **Key Insights**:
  -  The Aircraft Make like Boeing and Piper,Cessna commercial flights had destroyed and substantial damage, correlating with the highest injury rates.  
  - Severe damage leads to greater financial losses due to higher repairand replacement costs and legal liabilities.
  

### **4. Marketability Analysis**
#### **Aircraft Category, Purpose of Flight, and Country**
- **Objective**: To analyze the market demand and performance across different countries and the purposesof the flight.  
  **Key Insights**:
  - General aviation has higher accident rates and correlates with personal and commercial use in the countries.  
  - Commercial aircraft in the USA showed the highest injury count, a higher accident rate and higher marketability due to safety perception.
 - Recreational flights have more amateur-built aircraft, reducing perceived reliability.

### Recommendations
Investing in the aviation market requires careful analysis of safety, operational efficiency, financial performance, and market trends. Below are recommendations for potential investors based on insights derived from aviation data analysis:

### **1. Safety Recommendations**  
- **Invest in Advanced Weather Predicting Systems**:Support operators or manufacturers that incorporate advanced weather forecasting tools and onboard safety technologies.  
- **Focus on Modern Fleets**: Prioritize companies operating newer aircraft models with improved safety features.  

### **2. Operational Efficiency Recommendations**  
- **Professional Fleet Investment**: Avoid companies relying heavily on amateur-built aircraft to minimize operational risks.  
- **Multi-Engine Aircraft Preference**: Invest in operators focusing on multi-engine aircraft for greater safety and operational reliability.  
- **Efficiency in Ground Operations**: Support companies reducing turnaround times and optimizing resource allocation for stable operations.  

### **3. Marketability Recommendations**  
- **Commercial Over General Aviation**: Focus on commercial operators in regulated markets to capitalize on perceived safety and reliability.  
- **Market-Specific Investments**: Support airlines expanding into high-demand regions like Asia-Pacific for better growth prospects.  
- **Premium Offerings and Niche Markets**: Invest in companies providing premium services or catering to specialized markets like private charters.  

### **4. Financial Performance Recommendations**  
- **Focus on Reliable Manufacturers**: Avoid investing in operators using older or damage-prone aircraft models.  
- **Diversified Revenue Streams**: Choose companies with auxiliary income sources, such as cargo services or airport operations.  
- **Fuel Efficiency and Cost Control**: Invest in operators adopting fuel-efficient aircraft to reduce operational costs and enhance profitability.  




