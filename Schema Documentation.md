## Database Schema Documentation
## CURRENT_WEATHER
Stores daily weather data from the Open‑Meteo API including temperature, wind speed, precipitation, UV index, and daylight duration.
Primary Key: WEATHER_ID

| Column | Type | Key | Description |
| --- | --- | --- | --- |
| WEATHER_ID | INT | PK | Unique ID |
| WEATHER_DATE | DATE |  | Date of forecast |
| WEATHER_CODE | INT |  | Weather condition code |
| MAX_TEMP | FLOAT |  | Maximum temperature |
| MIN_TEMP | FLOAT |  | Minimum temperature |
| MAX_WIND_SPEED | FLOAT |  | Maximum wind speed |
| UV_INDEX | FLOAT |  | UV index |
| MAX_PRECIP_PROB | INTEGER |  | Maximum precipitation chance |
| DAYLIGHT_DURATION | FLOAT |  | Daylight duration (seconds) |
| SUNRISE | TIME |  | Sunrise time |
| SUNSET | TIME |  | Sunset time |
| CREATED_AT | TIME |  | Timestamp |

## RESTAURANT
Stores restaurant data for Louisville including name, location, cuisine, patio info, price level, and kid‑friendliness.
Primary Key: RES_ID

| Column | Type | Key | Description |
| --- | --- | --- | --- |
| RES_ID | INT | PK | Unique identifier |
| RES_NAME | TEXT |  | Restaurant name |
| RES_NEIGHBORHOOD | TEXT |  | Neighborhood area |
| RES_CUISINE | TEXT |  | Cuisine type |
| HAS_PATIO | BOOLEAN |  | Whether the restaurant has one |
| PATIO_TYPE | TEXT |  | Type of patio |
| LAT | FLOAT |  | Latitude |
| LONG | FLOAT |  | Longitude |
| PRICE_LEVEL | INT |  | Price level (1–4) |
| KID_FRIENDLY | BOOLEAN |  | Kid‑friendly indicator |
| CREATED_AT | TIME |  | Timestamp |


## PATIO_SCORES
Stores calculated comfort scores for patio dining and the reason for the score.
Has a 1:M relationship with both RESTAURANT and CURRENT_WEATHER.

Primary Key: SCORE_ID  
Foreign Keys: RES_ID, WEATHER_ID

| Column | Type | Key | Description |
| --- | --- | --- | --- |
| SCORE_ID | INT | PK | Unique score identifier |
| RES_ID | INT | FK | Restaurant identifier |
| WEATHER_ID | INT | FK | Weather identifier |
| COMFORT_SCORE | FLOAT |  | 0–100 patio comfort index |
| REASON | TEXT |  | Explanation of score |
| TIMESTAMP | TIME |  | Timestamp |

