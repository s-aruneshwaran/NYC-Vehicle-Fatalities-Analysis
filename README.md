# NYC Vehicle Fatalities Analysis 🚗📊

This project analyzes **New York City motor vehicle collision data** to understand patterns in **fatal traffic crashes across the five NYC boroughs**.

The goal is to identify **borough-specific contributing factors and geographic crash patterns** in order to support **targeted, data-driven road safety interventions.**

This project was completed as part of the **Explorer Transportation Data Science Project (TDSP)** organized by the **National Student Data Corps (NSDC)** in collaboration with the **U.S. Department of Transportation Federal Highway Administration** and the **Northeast Big Data Innovation Hub**.

---

# Project Objectives

The objectives of this project are:

- Perform **data cleaning and preprocessing**
- Conduct **exploratory data analysis (EDA)**
- Identify **fatal crash patterns across NYC boroughs**
- Analyze **contributing factors responsible for fatalities**
- Visualize **fatal crashes using geospatial mapping**
- Compare **fatality distribution across boroughs**
- Provide **data-driven recommendations for improving road safety**

---

# Dataset

Dataset: **NYC Open Data – Motor Vehicle Collisions – Crashes**

Each record represents a **reported motor vehicle crash in New York City** and includes details such as:

- Crash date and time  
- Borough location  
- Latitude and longitude  
- Contributing factors to the crash  
- Vehicle types involved  
- Number of injuries and fatalities  

Dataset Source:  
NYC Open Data – Motor Vehicle Collisions Dataset

Time range analyzed in this project:

**2014 – 2022**

---

# Tools and Libraries

The following Python libraries were used in this project:

- **Pandas** – Data cleaning and data manipulation  
- **NumPy** – Numerical operations  
- **Matplotlib** – Data visualization  
- **Seaborn** – Statistical plots and charts  
- **Folium** – Geospatial mapping and heatmaps  

---

# Project Workflow

## 1 Data Preparation

Steps performed:

- Loaded the NYC crash dataset
- Explored dataset structure using `head()` and `info()`
- Identified and handled **missing values**
- Filtered the dataset for **fatal crashes**
- Removed records without borough information

Key step:

```python
fatal_crashes = data[data['NUMBER OF PERSONS KILLED'] > 0]
```

This allowed the analysis to focus specifically on **fatal traffic incidents**.

---

# 2 Exploratory Data Analysis

## Fatalities by Borough

The analysis shows significant variation in traffic fatalities across boroughs.

**Brooklyn and Queens account for the majority of fatalities**, together representing over **60% of all traffic deaths** in the dataset.

This suggests that **traffic safety challenges differ across boroughs**.

---

## Top Contributing Factors

Fatal crashes were analyzed based on **contributing factors**.

Common causes include:

- Driver Inattention / Distraction
- Failure to Yield Right of Way
- Unsafe Speed
- Traffic Control Disregarded

Key insight:

Different boroughs show **different dominant crash causes**, suggesting that **targeted safety strategies are needed rather than a single city-wide policy**.

---

# 3 Borough-Specific Fatal Crash Analysis

A borough-level comparison was performed to understand how fatal crashes differ geographically.

Key findings:

- **Brooklyn** – Highest number of traffic fatalities  
- **Queens** – Large number of fatal crashes linked to intersection violations  
- **Manhattan** – Higher concentration of crashes involving vulnerable road users  
- **Bronx** – Moderate fatal crash levels  
- **Staten Island** – Smaller total crashes but higher influence of **speed-related incidents**

This highlights that **each borough has a unique crash pattern or "crash signature."**

---

# 4 Geospatial Analysis

Geospatial visualizations were created using **latitude and longitude coordinates**.

## Crash Density Heatmap

A heatmap was generated to show **high-density crash locations across New York City**.

Key observation:

Crash density is **highest in Manhattan and surrounding urban centers**, where traffic volume and pedestrian activity are significantly higher.

---

## Crash Severity Mapping

Crashes were mapped with markers to distinguish between:

- **Fatal crashes**
- **Injury crashes**

Different shapes and markers were used to improve **visual accessibility**.

This visualization helps identify **high-risk traffic zones**.

---

# 5 Research Question

The central research question of this project is:

**How do the number of fatalities and their contributing factors vary across the five New York City boroughs (Manhattan, Brooklyn, Queens, Bronx, and Staten Island)?**

---

# Key Findings

Major insights from the analysis include:

- **Brooklyn and Queens account for the majority of NYC traffic fatalities**
- **Each borough has distinct contributing crash factors**
- **Intersection violations are common in Queens**
- **Speed-related crashes are more prominent in Staten Island**
- **Crash density is highest in Manhattan**
- A large number of fatal crashes are labeled as **"Unspecified"**, indicating a **data collection gap**

---

# Recommendations

Based on the findings, several **borough-specific safety interventions** are recommended.

### Brooklyn

Focus on **reducing distracted driving** through awareness campaigns and enforcement.

### Queens

Improve **intersection safety** through better signal enforcement and road design.

### Manhattan

Increase protections for **pedestrians and cyclists**, including improved crossings and dedicated bike lanes.

### Staten Island

Implement **speed reduction measures**, including traffic calming and stricter enforcement.

### City-Wide

Improve **crash reporting and data collection** to reduce the number of **"Unspecified" contributing factors**.

---

# Project Structure

```
NYC-Vehicle-Fatalities-Analysis
│
├── certificate
│   └── ARUNESHWARAN SIVAKUMAR Explorer TDSP Certificate of Completion.pdf
│
├── data
│   └── README.md
│
├── notebooks
│   └── Explorer TDSP - ARUNESHWARAN SIVAKUMAR.ipynb
│
├── visualizations
│   ├── fatalities_by_borough.png
│   ├── contributing_factors_by_borough.png
│
├── maps
│   ├── Heatmap.png
│   ├── severity.png
│
├── poster
│   └── ARUNESHWARAN SIVAKUMAR Explorer TDSP Poster.pdf
│
├── README.md
```

---

# Project Poster

A **research poster** summarizing this project was created as part of the **Explorer Transportation Data Science Project (TDSP)**.

The poster highlights:

- Research objective
- Data analysis methodology
- Key visualizations
- Borough-level crash insights
- Data-driven safety recommendations

The poster can be found in the `poster/` folder of this repository.

---

# Acknowledgments

I would like to thank:

- **U.S. Department of Transportation Federal Highway Administration**
- **Northeast Big Data Innovation Hub**
- **National Student Data Corps (NSDC)**
- **NYC Open Data**

Their resources, dataset, and educational materials made this project possible.

---

# Author

**Aruneshwaran Sivakumar**  
Master's in Data Science  
Illinois Institute of Technology
