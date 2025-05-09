# 🕵️‍♂️ Los Angeles Crime Data Analysis (2020–2025)

This repository contains a comprehensive data analysis project on crime in Los Angeles, California, using data provided by the Los Angeles Police Department (LAPD). The dataset spans five years (2020 to 2025) and provides insights into crime patterns and trends across the city.

> 🔁 **Data Transformations:** Yes — major transformations were carried out using Power Query and SQL.

---

## 📌 Project Background

The LAPD sought an in-depth overview of crime data for the years 2020 through 2025 — the period since they began collecting consistent digital records. The primary goal of this analysis is to help the LAPD enhance public safety and optimize policing strategies in Los Angeles.

> 👉 **[Click here to interact with the Power BI Report](#)**

---

## 📊 Overview of the Data

The dataset was originally downloaded as a CSV file from [data.gov](https://data.gov), containing a single table with a unique identifier column `DIrec_No` for each crime entry. It was first imported into a **local MySQL server**, where appropriate data types were assigned to each column before further processing.

### ✅ Key Data Transformations (Power Query Editor)
The following transformations were applied:
- *(To be listed based on actual steps taken — e.g.,)*
- Removed duplicate records
- Filtered out null and blank rows
- Standardized column names and formats
- Replaced or corrected inconsistent values
- Extracted time-based features (year, month)
- Joined with external tables for enriched analysis

### 📂 Original Columns in the LA Crime Table
At the time of import into SQL, the dataset included the following columns:
- *(List to be completed — e.g.,)*
- DIrec_No
- Crime Date
- Reporting Area
- Weapon Used
- Premise Description
- Victim Demographics
- Crime Code Description
- Status

> 📎 **Note:** Due to the size of the main table, its CSV file was not uploaded. You can [download it here](#). However, scripts and sample CSVs generated from Power Query transformations are available in this repository.

---

## 🛠 Tools and Technologies Used

| Tool               | Description |
|--------------------|-------------|
| **Power BI**        | Core tool used for data visualization and dashboard creation. Power BI Service was used to publish and create a shareable web link. |
| **Power Query Editor** | Used within Power BI for cleaning and transforming the dataset (e.g., formatting, replacing values, removing duplicates). |
| **MySQL**           | Hosted the cleaned version of the data, which was then connected to Power BI for efficient querying and automatic refreshes. |
| **Microsoft Excel** | Used at the early stage of the project to understand data structure and guide the cleaning and modeling processes. |

---

## 🔄 Project Workflow

Establishing a clear workflow ensured that the project followed an organized, goal-aligned approach. Here's the general sequence followed:

1. **Define the Problem** — LAPD needs to understand recent crime trends.
2. **Data Collection** — Obtain raw crime data (2020–2025) from data.gov.
3. **Data Cleaning & Preparation** — Remove duplicates, standardize values, and enhance structure using SQL and Power Query.
4. **Data Modeling** — Build a relational model in Power BI to enable insights.
5. **Analysis & Visualization** — Visualize key trends by time, location, crime type.
6. **Insight Generation** — Provide data-driven recommendations for LAPD.

---

## 🎯 Project Objective

The main goal of this project is to analyze crime trends across the 21 LAPD areas from 2020 to 2025. By doing this, we aim to uncover patterns and insights that will assist the LAPD in improving its response and service to the Los Angeles community.

---

## 📥 Data Collection

The crime dataset was sourced from [data.gov](https://data.gov) and included:
- Crime event dates
- Crime types and codes
- Victim and suspect information
- Vehicle-related details
- Area and location data

---

## 🧹 Data Cleaning & Preparation

Initial cleaning was performed using **SQL**, where operations included:
- Removing duplicates
- Standardizing column formats
- Dropping irrelevant fields
- Creating new fields (e.g., Year, Month, Area Code)

Additional transformations were done in **Power Query Editor** before loading into Power BI.

---

## 🧩 Data Model

The Power BI **data model** was automatically generated and adjusted to define the correct relationships and cardinalities among the tables. This enabled efficient querying and slicing of the dataset by dimensions such as date, area, crime category, and more.

---

## 📈 Data Analysis & Visualization

The Power BI dashboard contains interactive visuals that explore:

## 📊 Overview
![Alt text](main/1st.png)


A total of over one million crimes—precisely 1,005,198—were recorded across the 21 areas of Los Angeles. Among these areas, Central stood out with the highest number of incidents, highlighting it as a focal point of concern. The average age of victims across all reported crimes was 29 years, showing that young adults continue to be the most vulnerable group.

Crimes occurred most frequently during the night period across all 21 locations, suggesting that this time frame remains the most unsafe for residents. Although the city has experienced a decline in crime rates from mid-2023 to 2025, the year-on-year (YoY) change still sits at 8.09%, which shows that the scale of incidents remains significant despite recent progress.

In terms of specific areas, the Central station recorded the highest volume of crime reports at around 70,000, followed by the 77th Street station with approximately 62,000 reports. Other stations that featured prominently in the top five include Pacific with 60,000 reports, Southwest with 58,000, and Hollywood with around 52,000 reports.

## 🧍 Victim Demographics

Looking into victim demographics by gender, out of the total number of reported crimes, 40.18% involved male victims, while 35.67% were female. A significant 24.14% of the cases had no gender identified for the victim, which could point to reporting limitations or cases where data wasn't fully captured.

When analyzed by age, victims between the age of 20 to 39 experienced the highest number of crimes, with 375,000 cases recorded. In contrast, victims aged 80 and above were the least affected, with only about 8,000 cases. Other age categories also recorded substantial numbers: victims aged 19 and below accounted for 311,000 cases, those between 40 to 59 years old were involved in 228,000 incidents, and the 60 to 79 age group experienced 83,000 crimes. The data paints a clear picture that the younger and working-age population is at the center of most victimizations.

On the subject of victim descent, individuals identified as Hispanic or Latino had the highest crime report figures, totaling 296,437. Reports involving victims of unknown descent followed closely at 251,495. White victims accounted for 201,451 cases, while Black victims were involved in 135,823. Other descent categories showed lower figures: 78,010 for other specified groups, 21,340 for those of other Asian descent, 5,991 for Korean descent, 4,838 for Filipino, 4,631 for Chinese, and 1,586 for Japanese. These figures reflect a mix of reporting accuracy and the city’s diverse population landscape.

## 🕵️ Crime Breakdown

Analyzing the trend of crime reports by year, there was a steady rise in incidents from 2020 up until the middle of 2022. However, from that point on, a noticeable decline has been observed, continuing through to 2025. This suggests that certain enforcement or community strategies may have started to take effect post-2022.

In terms of when crimes occur, most incidents happened during the night and afternoon periods, with 255,000 and 251,000 cases respectively. Evening and morning periods also recorded high, but slightly lower, numbers at 215,000 and 212,000 respectively. This trend highlights the need for heightened vigilance during key active hours, especially after dark and in the later part of the day.

Seasonal patterns also appear to influence crime activity. January emerged as the month with the highest crime reports, whereas December saw the lowest. This variation may reflect social behavior shifts tied to seasonal events, holidays, or other environmental factors.

## 📍 Crime Snapshots

When it comes to locations, the top five crime hotspots were found to be streets, single-family dwellings, multi-unit dwellings, parking lots, and other types of businesses—listed in descending order. This indicates that both public and residential spaces are especially prone to crime, pointing toward potential improvements in neighborhood security and public surveillance.

For police stations, the top five locations for crime reports remained consistent with earlier data, with Central, 77th Street, Pacific, Southwest, and Hollywood taking the lead. These stations are evidently the busiest in terms of criminal activity and may require additional resources or support to keep up with the volume of cases.

As for crime types, the most frequently reported offenses were vehicle theft, simple battery (assault), burglary from a vehicle, identity theft, and vandalism. These reflect a mix of property crimes and personal safety concerns, particularly related to mobility and public behavior.

The top five weapons used in these crimes were listed as unknown (suggesting either lack of witness clarity or reporting gaps), strong arm (use of physical force), another form of unknown weapon, verbal threat, and handguns. The dominance of “unknown” in weapon type also emphasizes data limitations or possibly the chaotic nature of many incidents.

## 📄 Crime Resolutions

Regarding how quickly crimes were reported, a large majority—about 70% of the 1,005,041 total crimes—were reported within 24 hours of occurring. However, some cases took longer to be reported: approximately 168,000 were reported between 2 to 7 days later, 40,000 were reported after 8 to 14 days, and 33,000 were reported between 15 to 30 days. Additionally, 32,000 incidents were reported within one to three months, and another 27,000 were only reported after three months had passed. These delays could reflect the nature of the crime, trauma, or accessibility of reporting mechanisms.

In terms of resolution status, about 80% of all reported cases are still under investigation, showing the scale of ongoing law enforcement effort. Beyond that, 109,225 cases fall under a category labeled “adult other,” and 86,877 cases have led to adult arrests. Juvenile arrests stood at 3,249, while 1,864 crimes were tagged as “juvenile other.” Lastly, 7% of all reported crimes currently have an unknown status, pointing to cases that may be either stalled or lacking sufficient evidence.



> 🔗 *Click [here](#) to explore the dashboard.*

---

## ✅ Conclusion

This analysis provides a valuable foundation for LAPD to understand crime distribution across Los Angeles. With it, the department can take strategic steps to better allocate resources and engage communities effectively.

---

## 📌 Recommendations
--

## 📌 Key Recommendations with Supporting Insights

### 1. 🚓 Resource Allocation & Hotspot Policing

**Recommendation:**  
Deploy more officers, surveillance tools, and response resources to the **Central, 77th Street, Pacific, Southwest, and Hollywood** divisions.

**Supporting Insight:**  
> Central reported ~70,000 crimes, 77th Street ~62,000, Pacific ~60,000, Southwest ~58,000, and Hollywood ~52,000—marking them as the top five stations for crime volume.

---

**Recommendation:**  
Increase night-time patrols citywide, especially around high-risk locations such as **streets, residential areas, and parking lots**.

**Supporting Insight:**  
> Most crimes occurred at **night (255k)** and **afternoon (251k)** hours. Streets, single-family dwellings, and parking lots were the top locations for incidents.

---

**Recommendation:**  
Temporarily reallocate resources during **January**, when crime peaks, and optimize coverage during **December**, which shows the lowest activity.

**Supporting Insight:**  
> January consistently had the **highest crime count**, while December recorded the **lowest**, suggesting seasonal variation in criminal activity.

---

### 2. 🧍 Community Engagement & Victim Support

**Recommendation:**  
Initiate targeted community outreach and safety campaigns for individuals aged **20–39 years**, who form the bulk of crime victims.

**Supporting Insight:**  
> 375,000 crimes were recorded against people aged **20–39**, the highest among all age groups.

---

**Recommendation:**  
Strengthen collaboration with **Hispanic/Latino communities** via multilingual initiatives, public forums, and safety training.

**Supporting Insight:**  
> Hispanic/Latino individuals accounted for the **largest share of victims (296,437)**, followed by unknown descent (251,495), White (201,451), and Black (135,823).

---

**Recommendation:**  
Improve gender data collection at the point of reporting and during investigations.

**Supporting Insight:**  
> **24.14%** of all crime records had **no gender identified**, limiting demographic-specific responses and intervention planning.

---

### 3. 📋 Data Quality & Reporting Improvements

**Recommendation:**  
Upgrade reporting systems and officer training to reduce the frequency of **"unknown" weapon types** and **unknown victim details**.

**Supporting Insight:**  
> The **most common weapon categories** were “unknown,” followed by strong-arm force and verbal threats. High "unknown" rates also appeared in victim gender and descent.

---

**Recommendation:**  
Encourage standardization and automation in data entry to minimize inconsistency.

**Supporting Insight:**  
> Over 250k victims were listed under **"unknown descent,"** and ~7% of cases had **unknown status**—indicating potential reporting or tracking issues.

---

### 4. 🏘️ Crime Prevention & Neighborhood Safety

**Recommendation:**  
Enhance environmental security measures such as **lighting, surveillance cameras, and patrols** in residential and public areas.

**Supporting Insight:**  
> Top crime locations: **streets, single-family homes, multi-unit dwellings, parking lots**, and businesses.

---

**Recommendation:**  
Conduct public awareness campaigns on property crime prevention, focusing on **vehicle theft**, **identity theft**, and **vandalism**.

**Supporting Insight:**  
> Most frequent crimes: **vehicle theft, simple battery, burglary from vehicle, identity theft**, and **vandalism**—many of which can be mitigated through citizen education and situational awareness.

---

### 5. ⏱️ Reporting Timeliness & Investigation Backlog

**Recommendation:**  
Promote and improve easy-access, anonymous, and **mobile-friendly crime reporting** tools.

**Supporting Insight:**  
> While **70% of crimes** were reported within **24 hours**, over **300,000 cases** were reported late (ranging from 2 days to 3+ months).

---

**Recommendation:**  
Invest in additional **detective units and digital tools** to address the backlog of unresolved cases (especially non-violent ones).

**Supporting Insight:**  
> **80% of cases** remain under investigation. Only **~86,000 adult arrests** and **~3,200 juvenile arrests** were made out of **1 million+ reports**.

---


## 🧠 Conclusion

Though progress has been made, **LAPD must continue prioritizing high-crime zones**, reinforce **data integrity**, and work closely with **affected communities**. These strategic actions can ensure a safer Los Angeles through both proactive prevention and responsive law enforcement.


