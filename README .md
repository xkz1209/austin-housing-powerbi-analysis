# Austin Housing Market Analysis | Power BI

**Interactive Dashboard & Real Estate Analytics Portfolio Project**

## Project Overview

This project explores **15,166 properties in the Austin, Texas area** through an interactive Power BI report. It combines a summary dashboard with location, school, and property-feature analysis to help users compare housing segments and investigate differences in listing prices.

The report addresses four business questions:

- What does the dataset reveal about typical home prices, property sizes, and housing composition?
- Where are properties located, and how can users explore homes within a selected price range?
- How do school-related characteristics vary across locations?
- Which property characteristics are associated with higher listing prices?
<img width="1455" height="785" alt="image" src="https://github.com/user-attachments/assets/fd5ab60f-d771-4c7d-95df-678529e844a8" />


## Tools & Technical Approach

| Area | Implementation |
|---|---|
| BI platform | Microsoft Power BI Desktop |
| KPI calculations | Custom DAX measures, including `Property Count`, `Median Home Price`, and `Average House Price` |
| Analytical tables | Housing facts, house attributes, location, schools, and property features |
| Dynamic analysis | Field parameters for switching property attributes and school groupings |
| Report navigation | Bookmarks and navigation buttons for four analytical views |
| Filtering | Expandable filter panel with numeric ranges and categorical slicers |
| Geographic analysis | Map visuals using property coordinates and ZIP codes |
| Explanatory analysis | Key Influencers visual for associations with listing price |
| Text exploration | Ranked listing-description words across price bands |

Additional measures support price-range selection, property coloring, dynamic school-chart titles, and the word-ranking display.

## Dataset & KPI Snapshot

The report uses an Austin-area housing dataset with listing prices, geographic coordinates, property characteristics, amenities, school-related attributes, and listing descriptions.

The following values reflect the supplied summary screenshot:

| Metric | Value |
|---|---:|
| Property count | 15,166 |
| Median listing price | $405,000 |
| Average listing price | $512,625 |
| Median living area | 1,975 sq. ft. |
| Median lot size | 8,276 sq. ft. |
| Single-family properties | 14,236 |
| Property types | 10 |

Prices are treated as **listing prices**, not verified transaction prices. These figures describe the project dataset and should not be interpreted as current Austin market statistics.

## Dashboard & Analytical Views

### 1. Summary

Provides an overview of housing composition and pricing through:

- KPI cards for property count, home prices, living area, and lot size.
- Property counts by home type, ZIP code, and construction year.
- Median versus average price comparisons across property types.
- Amenity prevalence, including cooling, heating, garages, spas, and views.

**Business use:** Establish a baseline before comparing narrower property segments.

### 2. Location

Maps Austin-area properties and provides a price-range selector for highlighting homes. Additional filters allow users to narrow the geographic analysis by property and location attributes.

**Business use:** Explore where properties meeting selected criteria are concentrated.

<details>
<summary>View location analysis</summary>

<img width="1456" height="778" alt="image" src="https://github.com/user-attachments/assets/93cc0a9b-055f-4edd-a18e-38161ccc4eac" />


</details>

### 3. Schools

Combines school-related KPI cards with a bubble map and ZIP-code comparisons. Users can switch between **school rating, school size, and students per teacher** to change the grouping used in the visuals.

**Business use:** Compare school-related characteristics alongside geographic housing options.

<details>
<summary>View school analysis</summary>

<img width="1456" height="779" alt="image" src="https://github.com/user-attachments/assets/650e24de-eb1d-421d-ad1b-5b79a56cc5a1" />


</details>

### 4. Features

Explores differences in listing prices through:

- Median-price comparisons for properties with and without selected amenities.
- A dynamic property-attribute selector, such as garage spaces.
- Key Influencers analysis of characteristics associated with higher prices.
- A matrix of frequently used listing-description words across price bands.

**Business use:** Identify property segments for further comparison and explore how listings are described at different price points.

<details>
<summary>View feature analysis</summary>

<img width="1452" height="784" alt="image" src="https://github.com/user-attachments/assets/fcca437c-1b5c-4950-8c52-49d24797a056" />


</details>

## Key Findings & Business Interpretation

| Area | Finding | Business Interpretation |
|---|---|---|
| Price distribution | Average price of **$512,625** exceeds the **$405,000** median by **$107,625**, or **26.6%** | The mean–median gap is consistent with higher-priced listings pulling up the average; use the median alongside the mean when describing a typical property. |
| Housing composition | **14,236 of 15,166 properties (93.9%)** are single-family homes | Overall results largely reflect this segment; compare other home types separately. |
| Common amenities | Approximately **98%** of properties have cooling and **99%** have heating | These amenities are common in this dataset and offer limited differentiation by presence alone. |
| Less common amenities | Approximately **8%** have a spa and **23%** have a view | These smaller segments merit closer price comparisons while accounting for property size and location. |
| Price associations | The displayed Key Influencers result associates **more than 4.5 bathrooms** with an approximately **$1.03M higher average listing price** versus the comparison group | Explore the characteristics of larger, higher-priced homes; this does not estimate the value added by installing bathrooms. |

Percentages for housing composition and the mean–median gap are calculated from the displayed totals. Amenity percentages and Key Influencers results are rounded values shown in the report. Results change with the filter context.

## Interactive Features

- **Bookmark navigation:** Switch between Summary, Location, Schools, and Features.
- **Expandable filter panel:** Show or hide detailed controls while preserving space for visuals.
- **Range filters:** Narrow listing price, living area, lot size, and construction year.
- **Categorical filters:** Explore home type, amenities, bedrooms, bathrooms, parking, location, and school characteristics.
- **Field parameters:** Switch analytical dimensions without adding separate charts for every attribute.

<details>
<summary>View the expanded filter panel</summary>

<img width="1104" height="683" alt="image" src="https://github.com/user-attachments/assets/a93f1014-b3e0-49f8-871b-29b788ccc68d" />


</details>

## Repository Contents

| File | Description |
|---|---|
| `housing_data_tutorial(3).pbix` | Power BI report and embedded data model |
| `README.md` | Project overview, analytical approach, findings, and usage notes |
| Five `.png` screenshots | Summary, Location, Schools, Features, and expanded filter panel previews |

The screenshot links above use the supplied image filenames. Keep these images in the same repository directory as this README, or update the links if you rename or move them.

## How to Explore the Project

1. Review the summary dashboard and expandable screenshots in this README.
2. Download `housing_data_tutorial(3).pbix` and open it in Power BI Desktop.
3. Use the left navigation buttons to explore the four analytical views. In Desktop editing mode, use **Ctrl + click** if required to activate a button.
4. Open the filter panel and adjust price, property, location, or school criteria.
5. Use the school and property-attribute selectors to compare different dimensions.

**Refresh note:** Refreshing requires access to the original source files and valid local source paths. The PBIX contains the saved data model; begin by exploring the saved report. Map rendering requires network access and may depend on Power BI settings. The supplied Location screenshot includes a legacy-map upgrade notice.

## Project Scope & Limitations

- This is a learning and portfolio project developed from a housing-analysis tutorial, not a production real estate service.
- The dataset is a historical sample; coverage and collection timing limit market-wide conclusions.
- Relationships between features and prices are descriptive associations, not causal estimates or a validated price-prediction model.
- Extreme recorded values, particularly lot sizes and living areas, warrant source validation before operational use. Median-based KPIs reduce sensitivity to extreme values but do not resolve data-quality issues.
- School metrics reflect attributes attached to housing records and should not be interpreted as independently weighted district-wide statistics.
- Business applications are potential uses of the analysis, not measured outcomes from implemented decisions.

## Skills Demonstrated

**Technical:** Power BI, DAX Measures, KPI Reporting, Field Parameters, Bookmarks, Slicers, Geographic Visualization, Key Influencers

**Analytical:** Housing Segmentation, Distribution Analysis, Feature Comparison, Geographic Analysis, Exploratory Text Analysis

**Business:** Translating business questions into interactive reporting, interpreting price differences, and communicating findings with appropriate limitations

---

**Author:** Jimmy Xu  
**Focus:** Business Analytics | Business Intelligence | Data Visualization
