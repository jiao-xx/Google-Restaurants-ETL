# Google-Restaurants-ETL

## Overview
This project focuses on extracting, transforming, and analyzing restaurants data in Toronto, Canada, using Google Cloud Platform (GCP). The workflow involves utilizing Google's APIs, Python, and Jupyter Notebook for ETL (Extract, Transform, Load) processes, storing and querying data in BigQuery, and finally visualizing insights using Looker Studio dashboards.

## Key Features
- Data Extraction: Utilized Google Maps API to collect detailed information on Chinese restaurants, including name, address, ratings, phone numbers, and website URLs.
- Data Transformation: Employed Python scripts to clean, format, and remove duplicate entries using Pandas within Jupyter Notebook.
- Data Storage and Querying: Loaded the processed data into BigQuery for efficient querying and analysis.
- Data Visualization: Designed interactive dashboards in Looker Studio to showcase key metrics such as average ratings, distribution of restaurants by rating, and contact details.

## Tools and Technologies
- Google Cloud Platform:
  - Google Maps API: To fetch raw data about restaurants.
  - BigQuery: For storing, querying, and managing data.
  - Looker Studio: For creating dynamic dashboards and visualizations.
- Python: For scripting and data cleaning (e.g., handling duplicates and formatting data).
- Jupyter Notebook: For developing and testing ETL pipelines.

## Workflow
1. **Extract**: 
   - Gathered data using the Google Maps API, including details like restaurant names, addresses, ratings, and phone numbers.

2. **Transform**:
   - Performed data cleaning in Python using Pandas:
     - Removed duplicate entries.
     - Standardized formatting of addresses and contact information.
   - Saved the cleaned dataset into a CSV format for further use.

3. **Load**:
   - Imported the cleaned dataset into BigQuery for structured storage and querying.

4. **Analyze and Visualize**:
   - Used SQL in BigQuery to generate insights, such as the distribution of restaurant ratings and clustering of top-rated restaurants by location.
   - Designed a dashboard in Looker Studio to present these insights in a visually appealing and interactive format.

## Results
The final output includes:
- A clean and structured dataset of restaurants in Toronto.
- A Looker Studio dashboard showcasing:
  - Average rating distribution.
  - Top-rated restaurants.
  - Contact details and locations.

### Sample Data Output:
| Name                          | Address                       | Rating | Phone Number    | Website                           |
|-------------------------------|-------------------------------|--------|-----------------|-----------------------------------|
| Hong Shing Restaurant         | 195 Dundas St W, Toronto, ON | 4.0    | (416) 977-3338 | http://www.hongshing.com/        |
| Spring China House            | 961 Eglinton Ave W, York, ON | 3.7    | (416) 780-0400 | http://www.springchinahouse.ca/ |

## Repository Structure
- **1. Googlemap.ipynb**: Extracts raw data from the Google Maps API.
- **2. Format.ipynb**: Cleans and formats the data.
- **3. Remove Duplicate.ipynb**: Removes duplicate entries to ensure data integrity.
- **Sample Screenshot**: Provides a visual representation of the final dataset.

## Future Enhancements
- Include additional data points such as customer reviews and cuisine types.
- Expand the project to include restaurants in other cities.
- Automate the entire ETL workflow using GCP tools like Cloud Functions and Cloud Composer.
