# UK Traffic Accident Analysis (2015-2018)

## Table of Contents
- [Introduction](#introduction)
- [ETL Process](#etl-process)
- [Data Documentation](#data-documentation)
- [Methodology](#methodology)
- [Analysis and Findings](#analysis-and-findings)
- [Visualizations](#visualizations)
- [Conclusions](#conclusions)

## Introduction
Road safety remains one of the most critical public health challenges in the United Kingdom, affecting thousands of lives annually through accidents, injuries, and fatalities. This comprehensive analysis examines traffic accident data from 2015 to 2018, seeking to understand the complex interplay of factors that contribute to road incidents and their severity. By analyzing over 529,294 accidents, this study provides crucial insights into patterns, risk factors, and potential intervention points for improving road safety.

### Research Objectives
- Identify temporal and seasonal patterns in accident occurrence
- Analyze the impact of environmental and road conditions
- Evaluate demographic patterns in casualties
- Assess vehicle-specific risk factors
- Develop evidence-based safety recommendations

## ETL Process

### 1. Data Validation and Structure Assessment
- Performed initial data comparison between redundant 2015 datasets
- Validated matching data between Data\RoadSafetyData_2015
- Confirmed 100% match for Accidents, Casualties, and Vehicles datasets
- Removed redundant 2015 folder after validation

### 2. File Structure Standardization
- Implemented consistent naming convention across datasets
- Renamed 2017 accident files from "ACC" to "Accidents_2017"
- Standardized Casualties files naming convention
- Updated Vehicles files from "Veh.csv" to standardized format

### 3. Data Transformation
- Converted all timestamps from UK to US format
- Resolved secondary time format issues
- Implemented additional validation checks

### 4. Data Cleaning
- Executed custom data cleaning script for:
  - Data standardization
  - Error correction
  - Format consistency
  - Generated comprehensive cleaning report

## Data Documentation

### Accident Severity Codes
| Code | Label |
|------|-------|
| 1 | Fatal |
| 2 | Serious |
| 3 | Slight |

### Weather Conditions
| Code | Label |
|------|-------|
| 1 | Fine no high winds |
| 2 | Raining no high winds |
| 3 | Snowing no high winds |
| 4 | Fine + high winds |
| 5 | Raining + high winds |
| 6 | Snowing + high winds |
| 7 | Fog or mist |
| 8 | Other |
| 9 | Unknown |
| -1 | Data missing or out of range |

### Road Type
| Code | Label |
|------|-------|
| 1 | Roundabout |
| 2 | One way street |
| 3 | Dual carriageway |
| 6 | Single carriageway |
| 7 | Slip road |
| 9 | Unknown |
| 12 | One way street/Slip road |
| -1 | Data missing or out of range |

## Methodology

### Dataset Overview
- Total Accidents: 529,294
- Fatal Accidents: 6,658
- Serious Accidents: 87,462
- Slight Accidents: 435,174

## Analysis and Findings

### 1. Temporal Analysis
- Peak accident times coincide with rush hours (7-9 AM and 4-6 PM)
- Highest severity rates occur during nighttime hours (11 PM - 4 AM)
- Early morning hours (2-5 AM) show lowest frequency but higher severity
- Weekend patterns differ significantly from weekday patterns

### 2. Weather Impact Analysis
- Adverse weather conditions significantly impact accident severity
- Rain associated with increased frequency but lower average severity
- Snow and ice show lower frequency but higher severity rates
- Clear weather accounts for majority of accidents due to higher traffic volume

### 3. Road and Speed Analysis
- Single carriageways account for highest number of accidents
- Higher speed limits correlate strongly with increased severity
- Urban roads show higher frequency but lower severity patterns
- Motorways show relatively low accident rates despite high speeds

## Conclusions and Recommendations

### Key Vulnerable Road User Groups
1. **Pedestrians**
   - Highest risk during urban rush hours
   - Children and elderly most vulnerable
   - Poor visibility in dark conditions increases risk

2. **Cyclists**
   - Urban intersection conflicts predominate
   - Limited visibility during peak hours
   - Lack of dedicated infrastructure

3. **Young Drivers (17-25)**
   - Inexperience in complex traffic situations
   - Night driving risks
   - Speed-related incidents

### Recommended Solutions
1. **Smart Infrastructure Implementation** (15-20% potential reduction)
   - AI-powered traffic management systems
   - Dynamic speed limits based on conditions
   - Connected vehicle infrastructure

2. **Enhanced Education Programs** (10-15% potential reduction)
   - Continuous learning systems
   - Virtual reality hazard training
   - Vulnerable user awareness training

3. **Technology-Based Solutions** (20-25% potential reduction)
   - Advanced driver assistance systems
   - Vehicle-to-vehicle communication
   - Automated emergency braking

### Expected Impact
Through this comprehensive approach, we project a potential reduction in overall accident rates by 30-40% over a five-year period. Success will require substantial government investment, public-private partnerships, and continuous monitoring and adaptation of strategies.

---
Project by Wolfrank Guzman  
[GitHub](https://github.com/guzmanwolfrank) | [Website](https://wolfrankguzman.com)
