## Business Problem
Louisville’s restaurant industry thrives on engagement from locals and tourists alike. Louisville has a variety of unique dining options offering different dining experience options like patios, rooftop seating, courtyards and indoor seating alike. However, Louisville also experiences changing weather that can make the comfort of outdoor dining vary leaving customers with a tough choice of where to dine. This app aims to simplify this decision and drive more people to eat at one of Louisville’s many restaurants.
## Data Sources
Weather Data
- Open Meteo

Restaurant Data
- compiled restaurant data from local restaurants, including location, cuisine type, price level etc
## Pipeline Architecture Overview
Extract
- Extract data from open meteo
Transform
- clean data, do validation checks, and compute patio comfort index
Load
- Load into 3 Supabase tables: weather table, restaurant table, and patio score
## Validation Checks
<img width="705" height="478" alt="image" src="https://github.com/user-attachments/assets/4c1ae886-ecb8-464a-b2e9-599a9f48330c" />
## Computing PCI
<img width="608" height="327" alt="image" src="https://github.com/user-attachments/assets/da40f39f-4f28-40ab-9405-19519bb33250" />

