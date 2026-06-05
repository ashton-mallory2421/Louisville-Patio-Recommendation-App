# Louisville-Patio-Recommendation-App
A Louisville Patio Recommendation App that uses Open Meteo API call to present weather data and recommend restaurants
# Louisville Patio Recommendation App - PowerBI
<img width="1458" height="806" alt="image" src="https://github.com/user-attachments/assets/e598e6b5-14de-4900-b120-52b796602b58" />
This interactive Power BI dashboard helps Louisville diners quickly decide whether it’s a great day to enjoy a patio and which restaurants offer the best outdoor options. It combines real‑time weather data, geospatial mapping, and restaurant attributes to deliver a simple, data‑driven dining guide.

# Purpose
The goal of the dashboard is to blend weather intelligence with local dining data to help Louisville residents and visitors make smarter, more enjoyable decisions about where to eat—especially when the weather is perfect for a patio.

# How it works
The dashboard makes a live call to the Open‑Meteo API to retrieve current and forecasted weather conditions for Louisville, including:
- Temperature highs and lows
- UV index
- Precipitation probability
- Sunrise and sunset times
- <img width="1433" height="802" alt="image" src="https://github.com/user-attachments/assets/9fb4cf5f-d0e2-43f2-a06c-8a7caa8d0b21" />

Using this data, the model computes a Patio Comfort Index (PCI) — a 0–100 score that summarizes how enjoyable outdoor dining will be. A higher PCI means better patio weather.
<img width="333" height="275" alt="image" src="https://github.com/user-attachments/assets/794fe1ec-d92f-4f9e-bc26-db2a992cd889" />

# Interactive Restaurant Map
A dynamic map plots restaurants across Louisville, categorized by patio type:
- Open patios
- Covered patios
- Indoor only
- <img width="582" height="260" alt="image" src="https://github.com/user-attachments/assets/996f188c-f6f0-4355-8e4a-641eadf68129" />

Users can filter the map and recommendation table by:
- Cuisine
- Price level
- Patio type
- Neighborhood
This makes it easy to explore options that match your preferences.
<img width="1160" height="652" alt="image" src="https://github.com/user-attachments/assets/f791e93e-c9ff-4cfc-8dc6-0b247eadcc88" />
# Recommendation Table
A sortable table lists curated restaurant recommendations with details such as:
- Neighborhood
- Cuisine
- Price level
- Whether a patio is available
- Patio type (Open, Covered, Indoor)
This gives users a quick way to compare and choose the best spot for the current weather.
<img width="636" height="303" alt="image" src="https://github.com/user-attachments/assets/5e2726ab-2b43-424f-9d3e-6d434cfd0599" />
