# Bank Loan Application Analysis & FTE Planning 📊

## Overview 🔍

This repository presents a comprehensive analysis of loan application data and staffing recommendations for efficient workforce management. Developed in the context of one of Australia's Big 4 banks, it leverages advanced time series forecasting techniques to uncover key patterns in application volumes and translates these insights into actionable FTE (Full-Time Equivalent) planning strategies.

## The Story of Our Data Journey 📖

### Chapter 1: Understanding Historical Patterns 📈

Our journey begins with exploring loan application volumes from September 2012 to August 2014:

![image](https://github.com/user-attachments/assets/07d1ec86-9240-49b4-97c7-0e116c7aa709)

- **Mid-year peaks**: May-July consistently show highest volumes, with July 2014 reaching 7,318 applications
- **Holiday dips**: December-January show lowest volumes (~4,700 applications), correlating with holiday periods
- **High variability**: Monthly volumes fluctuate by more than 2,500 applications within the same year
- **Growth trend**: 2014 peaks exceed 2013 levels, showing year-over-year growth
- **Quarterly cycles**: Applications build and decline quarterly, possibly aligned with business/reporting cycles

This historical analysis immediately suggests opportunities for resource allocation, system maintenance scheduling, and targeted marketing.

### Chapter 2: Geographical Insights 🗺️

![image](https://github.com/user-attachments/assets/517dd6dc-616e-4684-9e47-ac8b279365cf)

![image](https://github.com/user-attachments/assets/df7fcbd1-e442-4e53-a129-dae0651f6d26)

The geographical distribution reveals significant concentration:

- There's a significant east coast concentration, with Victoria and NSW combining for nearly two-thirds of all applications
- Queensland rounds out the top three with 16%. The top three states combined account for over 80% of all applications

These geographical patterns suggest focusing resources on east coast operations while exploring growth opportunities in Western and South Australia. Centralised processing can efficiently handle smaller territories (TAS, NT, ACT).

### Chapter 3: Understanding Loan Size Distribution 💰

![image](https://github.com/user-attachments/assets/492480db-25ce-4997-8dd2-cd667e35d589)

![image](https://github.com/user-attachments/assets/82e8991b-c7fb-4c36-8069-ca7feb9b9239)

Our analysis of loan amounts uncovers an interesting skewed distribution:

- Strong concentration at lower end: 51% under $50,000, 75% under $200,000
- Few large loans: Only 10% exceed $500,000, less than 1% exceed $1M
- Mean loan amount ($164,065) is more than triple the median ($50,000)

- High volume of smaller loans indicates strong small business lending orientation
- Few large loans (>$750K) represent disproportionate value, requiring enhanced assessment
- Potential to expand medium-sized offerings ($200K-$500K)
- The loan categories reveal diverse financing needs from Start up to rural loans

### Chapter 4: Forecasting the Future 🔮

Using SARIMA (Seasonal Autoregressive Integrated Moving Average) modelling, we forecast the next 12 months:

![image](https://github.com/user-attachments/assets/8b1eb7b0-c523-4f72-991b-60503dbe1ad9)

- Total volume reaches 74,407 applications (September 2014 to August 2015)
- Monthly applications average 6,201 across the forecast period
- Overall growth shows a 2.7% increase from the previous year
- July 2015 represents the peak and January 2015 shows the lowest volumes
- The forecast maintains the seasonal patterns observed historically
- Forecast accuracy achieves 5.25% MAPE on historical data enabling confident resource planning and optimised staffing levels

### Chapter 5: Transforming Insights into Action 🎯

Based on our forecast, we developed comprehensive FTE planning recommendations:

![image](https://github.com/user-attachments/assets/5a9fab18-8867-4888-9fc9-90ea400925fb)

#### Short-term Tactical Actions:

**Leave Management:**
- Encourage leave utilisation during surplus months (Sep-Feb)
- Restrict non-essential leave during deficit months (May-Jul)
- Plan training and development activities during Q4 2014

**Workload Distribution:**
- Implement "work ahead" strategies during surplus months
- Consider processing simpler applications during lower volume periods
- Adjust service level agreements during peak periods if necessary
- Plan for targeted overtime during peak months

#### Strategic Actions:

**Workforce Structure:**
- Maintain the core 85 FTE team as it's well-balanced for annual requirements
- Develop a flexible workforce component (15-20% of base) through cross-trained staff and temporary workers

**Process Improvements:**
- Identify opportunities to reduce handle time, especially for simpler applications
- Review and streamline approval processes for peak periods
- Invest in automation tools to reduce manual processing time

**Capacity Flexibility:**
- Implement staggered shifts during peak periods to extend operating hours
- Consider work-from-home options to increase flexibility
- Explore outsourcing options for simple applications during peaks

**Long-term Recommendations:**
- Explore options to smooth application volumes through the year with targeted marketing

## The Benefits 💼

Our recommended approach delivers four key benefits:
- **Optimal cost-to-service ratio**: Balancing permanent and flexible resources
- **Higher customer satisfaction**: Maintaining service levels even during peak periods
- **Elasticity to handle volume spikes**: Creating flexible capacity when needed
- **Sustainable, predictable operations**: Building a more stable system

## Technical Implementation 🛠️

The analysis uses a SARIMA time series forecasting approach, implemented in Python. The repository includes:
- Data preprocessing scripts
- Time series decomposition
- SARIMA parameter optimization
- Forecast generation

## Applications 🗃️
This analysis framework can be valuable for:

- Resource planning teams
- Operations management
- Business forecasting
- Budget planning
- Capacity management
