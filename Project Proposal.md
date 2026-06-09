## Louisville Weather Restaurant Patio Recommender Project Proposal
Developer: Ashton Mallory
Target Audience: Louisville KY food enthusiasts, residents and tourists
Technology stack: Python, Supabase, PowerBI, Open-Meteo API
## Background:
This project proposes an interactive weather application that will provide users with restaurant recommendations based on a variety of weather factors and forecasted comfort conditions. This app will use Open-Meteo API to retrieve real time weather data and recommend restaurants and patios that best match the current and forecasted comfort conditions.  
## Business Problem
Louisville’s restaurant industry thrives on engagement from locals and tourists alike. Louisville has a variety of unique dining options offering different dining experience options like patios, rooftop seating, courtyards and indoor seating alike. However, Louisville also experiences changing weather that can make the comfort of outdoor dining vary leaving customers with a tough choice of where to dine. This app aims to simplify this decision and drive more people to eat at one of Louisville’s many restaurants.
## Objectives:
-	Pull real time weather data from Open-Meteo API for Louisville, KY
-	Use Python to clean data and store in a Supabase Database
-	Develop a Patio Comfort Index measure to score outdoor dining suitability
-	Build a web-based weather and recommendation application using Dash
-	Recommend restaurants based on weather, user preferences and patio conditions
## Technical Approach:
Data Source
-	Open Meteo API
-	Parameters: temperature, humidity, precipitation, wind speed, weather code, UV index
Tools and Technologies
-	Python (requests, pandas)
-	PowerBI
-	Supabase for storage
ETL Workflow
1.	Extract
-	API call to Open-Meteo
- Load restaurant data from CSV
2.	Transform
  - Clean data
  - Compute Patio Comfort Index
3.	Load
-	Cleaned and structured data goes into Supabase
  -	Feed data into dashboard
## PCI Calculation:
The PCI calculation is calculated using the formula below:
    - pci = 100
    - pci -= abs(75 - temp) * 1.0
    - pci -= max(0, wind - 8) * 1.0
    - pci -= precip * 0.5
    - pci -= max(0, uv - 6) * 2.0
    - return max(0, min(100, pci))

## Visualization Strategy:
-	Current weather summary card
-	Daily Forecast
-	Geographical Analysis
-	PCI score chart and visualization
-	Restaurant recommendation list with filters
## Diagram:
 <img width="975" height="482" alt="image" src="https://github.com/user-attachments/assets/d7e3486a-87da-4b7f-b4f9-cfc8bba245e6" />
## Timeline: 
- Week 1	Initial research, API selection, proposal draft
- Week 2	Build API extraction code and transformation pipeline
- Week 3	Complete storage layer and data cleaning
- Week 4	Build Dashboard and Visualization
- Week 5	Final testing, presentation and submission

## Expected Outcomes and Deliverables:
•	Interactive dashboard displaying weather data and restaurant/patio recommendations
•	Working ETL pipeline that requests data from Open-Meteo API, cleans the data and structures into tabular format, and then loads data into dashboard
•	Polished and professional presentation showcasing the final dashboard and its features

