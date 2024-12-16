# UK Traffic Accident Analysis (2015-2018)

## 📊 Project Overview
A comprehensive analysis of traffic accidents in the United Kingdom from 2015 to 2018, examining patterns, trends, and factors contributing to accident severity and frequency. This project combines data from multiple sources to provide insights into road safety and accident prevention.

## 🎯 Key Objectives
- Analyze temporal patterns in accident occurrence
- Identify factors influencing accident severity
- Examine relationships between weather conditions and accidents
- Study vehicle type involvement patterns
- Analyze casualty demographics
- Provide actionable insights for road safety improvement

## 📁 Data Sources
The analysis uses three primary datasets from the UK Department for Transport:
1. **Accidents Dataset**: Details of accident circumstances
2. **Casualties Dataset**: Information about individuals involved
3. **Vehicles Dataset**: Data about vehicles involved in accidents

## 📖 Data Dictionary

### Accidents Dataset
| Variable | Description | Type |
|----------|-------------|------|
| Accident_Index | Unique identifier for each accident | String |
| Date | Date of accident occurrence | Date |
| Time | Time of accident occurrence | Time |
| Location_Easting_OSGR | Easting coordinates | Float |
| Location_Northing_OSGR | Northing coordinates | Float |
| Longitude | Geographical longitude | Float |
| Latitude | Geographical latitude | Float |
| Police_Force | Recording police force | Category |
| Accident_Severity | Fatal/Serious/Slight | Category |
| Number_of_Vehicles | Count of vehicles involved | Integer |
| Number_of_Casualties | Count of casualties | Integer |
| Road_Type | Type of road | Category |
| Speed_limit | Posted speed limit | Integer |
| Weather_Conditions | Weather at time of accident | Category |
| Light_Conditions | Lighting conditions | Category |

### Casualties Dataset
| Variable | Description | Type |
|----------|-------------|------|
| Accident_Index | Links to accident record | String |
| Casualty_Reference | Unique casualty identifier | String |
| Casualty_Severity | Fatal/Serious/Slight | Category |
| Casualty_Type | Type of casualty | Category |
| Sex_of_Casualty | Gender | Category |
| Age_of_Casualty | Age in years | Integer |
| Age_Band_of_Casualty | Age group | Category |

### Vehicles Dataset
| Variable | Description | Type |
|----------|-------------|------|
| Accident_Index | Links to accident record | String |
| Vehicle_Reference | Unique vehicle identifier | String |
| Vehicle_Type | Category of vehicle | Category |
| Age_of_Vehicle | Years since first registration | Integer |
| Driver_Age | Age of driver | Integer |
| Engine_Capacity_(CC) | Engine size in CC | Integer |

## 🛠️ Technologies Used
- Python 3.7+
- Pandas for data manipulation
- Plotly for interactive visualizations
- Seaborn/Matplotlib for static visualizations
- HTML/CSS for report generation

## 📊 Visualizations
1. Accident Severity Trends
2. Temporal Pattern Analysis
3. Weather Impact Assessment
4. Vehicle Type Distribution
5. Casualty Demographics
6. Hour/Day Heatmaps
7. Road Type Analysis

## 🔍 Key Findings
1. **Temporal Patterns**
   - Peak accident times correlate with rush hours
   - Higher severity rates during night hours
   - Distinct weekend vs weekday patterns

2. **Weather Impact**
   - Adverse weather contributes to 20% of accidents
   - Rain increases frequency but not necessarily severity
   - Poor visibility conditions show higher severity rates

3. **Vehicle Factors**
   - Cars dominate accident statistics
   - Motorcycles show higher severity rates
   - Heavy vehicles involved in fewer but more severe accidents

4. **Demographic Insights**
   - Age-specific risk patterns identified
   - Gender distribution variations noted
   - Urban vs rural difference in casualty profiles

## 📈 Installation & Usage
```bash
# Clone the repository
git clone https://github.com/yourusername/uk-accident-analysis.git

# Install required packages
pip install -r requirements.txt

# Run the analysis
python accident_analysis.py
```

## 📁 Project Structure
```
uk-accident-analysis/
├── Data/
│   ├── Combined_Data/
│   │   ├── combined_accidents.csv
│   │   ├── combined_casualties.csv
│   │   └── combined_vehicles.csv
├── visualizations/
│   └── comprehensive_analysis.html
├── requirements.txt
├── accident_analysis.py
└── README.md
```

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## 📜 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments
- UK Department for Transport for providing the data
- Contributors and reviewers
- Open source community

## 📧 Contact
For questions or feedback, please contact [your-email@example.com]

---
**Note**: This is an analytical study using publicly available data. All findings should be cross-referenced with official sources for policy decisions.
