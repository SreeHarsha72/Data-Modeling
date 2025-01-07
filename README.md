# Data-Modeling

This repo demonstrates of creating a structured data model by showing how a large dataset containing taxi trip data (2009–2023) can be transformed from a flat file format into a dimensional model using Python and visualization tools like Lucidchart. 

### Overview of Data:
1. **Data Source**: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
2. **Data Columns**: Includes trip details (vendor ID, pickup/drop datetime, passenger count, trip distance, locations, rate codes, payment types, and charges).
3. **Data Dictionary**: https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf
4. **Objective**: Extract and understand the dataset's structure using a data dictionary.

### Steps
1. **Understanding Columns**: Review data and identify key columns for dimensional modeling.
2. **Dimensional Modeling**:
   - Create fact and dimension tables.
   - Dimension tables contain static/descriptive values (e.g., pickup/drop locations, rate codes, payment types).
   - Fact tables include transactional data (e.g., IDs, passenger counts, trip distances, fare amounts).
3. **Tools Used**:
   - **Lucidchart**: For designing the data model.
   - **Python (Pandas)**: To transform the flat file into the fact-dimension schema:
     - Convert datetime columns to proper formats.
     - Extract metadata (e.g., hours, months).
     - Drop duplicates and reset indices.
     - Map descriptive values (e.g., rate codes) using dictionaries.
4. **Code Implementation**:
   - Sequentially create and populate dimension tables.
   - Merge dimension tables into a fact table using common keys.
   - Validate the schema by outputting sample data.
  
!(data_model.jpeg)
