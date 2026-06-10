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

## Validation checks
<img width="708" height="498" alt="image" src="https://github.com/user-attachments/assets/ccdba4d2-8c7c-466a-9e0b-f7a3f40cb028" />

## PCI Calculation

<img width="598" height="337" alt="image" src="https://github.com/user-attachments/assets/07cb1315-863a-42ff-8d3c-7945aa281896" />

## Dashboard Demo
<img width="1305" height="730" alt="image" src="https://github.com/user-attachments/assets/9e27e46e-b2c5-4167-a974-a92a5aeb80b5" />
<img width="1298" height="737" alt="image" src="https://github.com/user-attachments/assets/c3334607-253f-4bdf-9d79-53b9e98b294f" />
<img width="1300" height="737" alt="image" src="https://github.com/user-attachments/assets/e5facfe8-f494-4fc4-9b49-04d66eadf9fc" />




