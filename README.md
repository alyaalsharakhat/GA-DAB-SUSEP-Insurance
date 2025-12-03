# SUSEP Auto Insurance Analysis (2017–2020)
Analyzing Brazil’s auto-insurance claims (2017–2020) to identify high-risk vehicles, drivers, and regions. Assessed claim frequency, severity, and loss ratios to support underwriting decisions.

## Overview
This project analyzes Brazilian auto insurance claims from 2017 to 2020 using SUSEP public data.
The goal is to identify high-risk vehicle segments, driver profiles, and regions by examining Number of Claims, Amount Paid, and Loss Ratio.
The insights support insurers in improving pricing, underwriting, and risk selection.

## Dataset
- Source: SUSEP (Brazil’s Federal Insurance Regulator)
- Years: 2017–2020
- Type: Aggregated insurance records (privacy-preserving)
- Link: [SUSEP Auto Insurance](https://www2.susep.gov.br/menuestatistica/autoseg/principal.aspx) 

## Data Cleaning
  - Merged multiple CSV files into a unified dataset.
  - Created derived fields: vehicle age, total claims, loss ratio, etc.
  - Handled missing values and inconsistencies.
  - Standardized categories for vehicle, driver, and region.
  - Exported to Tableau for visualization.

## Analysis
### 1. Number of Claims
  - Brands: Chevrolet, Volkswagen, and Fiat have the highest claim counts.
  - Top Models (from the top 8 Brannds): HB20, Honda Fit, Chevrolet Onix.
  - Vehicle Type (from the top Bramds and Models): Passenger–Domestic dominates total claims.
  - Vehicle Age: New and Recent vehicles report more claims.
  - Driver: Male drivers report more claims; age 55+ has the highest count, followed by 36–45.
  - Region: Southeast states (São Paulo and Rio de Janeiro) lead in claims due to high vehicle concentration.

### 2. Amount Paid
  - Brands: Chevrolet, Volkswagen, Fiat, Toyota drive the highest total payout.
  - Top Models: Toyota Hilux and Corolla.
  - Vehicle Type: Passenger–Domestic and Trucks have the largest payouts.
  - Vehicle Age: New and Recent vehicles generate the highest claim costs.
  - Region: São Paulo and Rio de Janeiro lead, followed by Minas Gerais and Rio Grande do Sul.
  - Driver: Male drivers generate more indemnity costs; age groups 36–45 and 55+ are top contributors.

### 3. Loss Ratio (Profitability)
  - Lada is the extreme outlier brand.
  - Model: Lada Laika SW 5p >500% loss ratio. 
  - Passenger–Imported and Passenger–Domestic segments have elevated loss ratios (~60–70%).
  - New and Recent vehicles have higher loss ratios; Very Old vehicles have the lowest.
  - Regions: Northeast states (Bahia, Piauí, Pernambuco, Tocantins) highest; Rio de Janeiro also high.
  - Driver: Male drivers (74%) higher than female (65%); middle-age groups (26–35, 36–45) highest.

## Conclusion 
### Combined Risk Segments
#### Consistently high-risk segments across all metrics
- Vehicle: Toyota, Passenger–Domestic, Recent vehicles
- Driver: Male, Age 36–45
- Region: Rio de Janeiro

### Outlier Risk Segment
  - Lada Laika SW 5p: loss ratio >500%, costing insurer 5x premium.
    
## Key Insights
  - Certain brands, models, and vehicle types dominate claims and payouts.
  - Male drivers and specific age groups pose higher risk.
  - Geographic concentration influences claims and profitability.
  - Extreme outliers like Lada Laika SW 5p require special attention.

## Recommendations
  - Increase premiums for high-risk vehicle segments.
  - Strengthen underwriting for high-risk drivers.
  - Apply territorial pricing adjustments.
  - Re-price or restrict outlier vehicles with extreme loss ratios.

## Tools & Libraries
  - Python: Pandas, NumPy, Jupyter Notebook
  - Tableau: Visualizations

## Project Structure
GA-DAB-SUSEP-Insurance

│

├── data/        # Link of the source data

├── notebooks/   # Python code

├── Presentation # The 

├── Report       # Technical Report

└── README.md


## Future Improvements
- Integrate additional years of SUSEP data.
- If could find a way to include more granular driver or vehicle data.


 
