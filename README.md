# Introduction

##  Overview

anzania, as a developing country, struggles with providing clean water to its population of over 57,000,000. There are many water points already established in the country, but some are in need of repair while others have failed altogether. According to the World Health Organization, access to safe and clean drinking water is essential for health, development, and well-being.

### Business understanding

The goal is to ensure that water wells in Tanzania are functional, providing reliable access to clean water for communities. Ensuring well functionality involves understanding various factors influencing the wells' status, such as management practices, payment methods, and water quality. Effective management and maintenance strategies can be developed by identifying key determinants of well functionality, leading to improved water access for the population..


## Problem statement
The primary problem is the high rate of non-functional water wells in Tanzania, which undermines efforts to provide safe and reliable water access. This project aims to identify the critical factors affecting well functionality, predict the status of wells using these factors, and recommend strategies to improve well management and maintenance.

## DATA UNDERSTANDING

The main data used from the project is from two datasets which have been merged.

The first dataset contained wells infomation and the second on contains information of wells condition

Main  data has 27813 rows × 27 columns

Our data gives information about the Tanzania wells and its features.

link: https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/data/

# Columns

1. **id**: Unique identifier, .
2. **amount_tsh**: .
3. **date_recorded**: .
4. **funder**:  funder of the  well.
5. **gps_height**: heiht of the well .
6. **installer**: installer of the well.
7. **longitude, latitude**:  geographical location of the well.
8. **wpt_name**: Name of the water point, .
9. **num_private**: .
10. **basin**: source of water.
11. **subvillage**: .
12. **region**: region the well is located.
13. **region_code**: Can be redundant with `region`.
14. **district_code**: .
15. **lga**: Local government area.
16. **ward**: .
17. **population**: population of the area.
18. **public_meeting**: 
19. **recorded_by**: 
20. **scheme_management**:management schemes.
21. **scheme_name**:.
22. **permit**:  permit status .
23. **construction_year**:.
24. **extraction_type**: How the water is sourced.
25. **extraction_type_group**: Can be redundant with `extraction_type`.
26. **extraction_type_class**: Can be redundant with `extraction_type`.
27. **management**: who manages the well.
28. **management_group**: Can be redundant with `management`.
29. **payment**: Relevant  payment types.
30. **payment_type**: Can be redundant with `payment`.
31. **water_quality**: 
32. **quality_group**: Can be redundant with `water_quality`.
33. **quantity**: Relevant for quantity analysis.
34. **quantity_group**: Can be redundant with `quantity`.
35. **source**: source of the well water.
36. **source_type**: Can be redundant with `source`.
37. **source_class**: Can be redundant with `source`.
38. **waterpoint_type**:
39. **waterpoint_type_group**: Can be redundant with `waterpoint_type`.
40. **status_group**: The target variable, important for analysis.

    ## EXPLORATORY DATA  ANALYSIS

#### 1. Distribution of Well Status (status_group)
![Genre Rating Relationship](https://github.com/dennis2440/dsc-phase-3-project/blob/main/files/download%20(8).png)

This plot shows the count of wells categorized by their status. It indicates the proportion of functional and non-functional wells.
Insight: There are more functional wells compared to non-functional ones.


#### 2. Distribution of Regions (region)
![Genre Rating Relationship](https://github.com/dennis2440/dsc-phase-3-project/blob/main/files/download%20(9).png)

This plot displays the number of wells in each region. It helps understand the geographical distribution of wells.

Insight : The regions with the highest number of wells are shown, with Iringa, Manyara, and Tanga being prominent

### Distribution of Management Types
![Genre Rating Relationship](https://github.com/dennis2440/dsc-phase-3-project/blob/main/files/download%20(10).png)

Some management types are more prevalent, potentially impacting the functionality rates of the wells they oversee.

### Distribution of payment types
![Genre Rating Relationship](https://github.com/dennis2440/dsc-phase-3-project/blob/main/files/download%20(11).png)

This plot shows the distribution of payment types used for accessing the wells. Different payment models might influence the maintenance and operational status of the wells.

### 5.Well Status by Water Quality
(![Genre Rating Relationship](https://github.com/dennis2440/dsc-phase-3-project/blob/main/files/download%20(12).png)

The plot explores the relationship between water quality and well status. Wells providing high-quality water might be better maintained, affecting their functionality.

There was also some Modelling done:
## Modelling Findings

Based on the analysis, the Random Forest model outperforms the Decision Tree and XGBoost models in terms of accuracy, precision, recall, F1 score,Therefore, Random Forest is recommended for predicting the functionality of water wells in Tanzania.

### Key Findings

- **Important Features:** Management practices, payment methods, and water quality are significant factors influencing well functionality.
- **Model Performance:** Random Forest model achieved the highest performance metrics, indicating its effectiveness in predicting well status.

## Conclusions and Recommendations
1.Focus on Effective Management: Promote and support management practices that correlate with higher well functionality.

2.Sustainable Payment Models: Encourage payment methods that ensure funds for regular maintenance, potentially improving functionality rates.
