# Aviation Accident Risk Analysis

## Overview

This project provides an in-depth analysis of historical aviation accident data to determine the lowest-risk aircraft for a company entering the commercial and private aviation sectors. By identifying trends in accident frequency across different aircraft makes, models, and operating conditions, this analysis aims to translate data-driven findings into actionable insights for strategic aircraft investment.

## Business Understanding

### Stakeholder
The primary stakeholder is the **Head of the new Aviation Division**, who is responsible for aircraft purchasing and operational risk management.

### Key Business Questions
1.  Which specific aircraft makes and models exhibit the lowest historical accident rates, qualifying them as the safest investment?
2.  Are there specific operational factors (e.g., time of year, weather) that significantly increase accident risk, and how can the company mitigate them?
3.  What actionable, data-backed recommendations can be provided to inform the initial fleet acquisition strategy?

## Data Understanding and Analysis

### Source of Data
The analysis utilizes the **Aviation Accident Data (`Aviation_Data.csv`)** dataset, which contains records of aviation incidents and accidents.

### Description of Data
* **Initial Size:** 90,348 entries and 31 columns.
* **Key Features:** Includes details on the aircraft's `Make` and `Model`, `Event.Date`, accident `Location`, and various metrics on injuries (`Total.Fatal.Injuries`, `Total.Uninjured`).
* **Preprocessing:** Data cleaning involved imputing missing numeric values (e.g., `Total.Fatal.Injuries`, `Number.of.Engines`) and removing remaining records with missing data, resulting in a clean dataset of **58,769 entries** for analysis.

### Three Key Visualizations

The following visualizations were used to explore risk factors in the data:

1.  **Top 10 Aircraft Makes by Accident Count**
    * **Visualization Description:** A bar chart illustrating the total number of accidents recorded for the ten most frequent aircraft manufacturers. 
    * **Insight:** Clearly demonstrates that certain manufacturers, such as **Cessna**, account for a disproportionately high volume of recorded accidents, while others like **Boeing** are significantly lower.

2.  **Total Accidents by Month**
    * **Visualization Description:** A line or bar chart plotting the total number of accidents across the 12 months of the year. 
    * **Insight:** Reveals a clear **seasonal pattern**, with a distinct peak in accident occurrences during the summer months, specifically **July**.

3.  **Total Accidents by Weather Condition (VMC vs. IMC)**
    * **Visualization Description:** A bar chart comparing the frequency of accidents that occurred under Visual Meteorological Conditions (VMC - clear weather) versus Instrument Meteorological Conditions (IMC - low visibility/adverse weather). 
    * **Insight:** Shows that the majority of accidents occur under VMC (clear weather), suggesting that factors like **human error** or poor decision-making, rather than environmental conditions, are the dominant risk drivers.

## Conclusion

The analysis successfully identified quantifiable risk profiles for aircraft investment and operational planning, providing the following key conclusions:

1.  **Aircraft Make Risk:** **Boeing** aircraft are recommended for investment due to their relatively lower accident frequency. Conversely, the high accident rate associated with **Cessna** models suggests a higher operational risk that must be approached with caution.
2.  **Seasonal Risk Mitigation:** Accident occurrences peak in **July**. The new division should schedule all major maintenance, safety audits, and operational stand-downs *before* and *after* this peak period to proactively minimize risk.
3.  **Focus on Human Factors:** Since most accidents occur in **clear weather (VMC)**, the primary focus for risk mitigation should be on enhanced pilot training, stricter adherence to Standard Operating Procedures (SOPs), and rigorous crew resource management to address human error.