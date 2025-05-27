# This is an end - to - end Data Analyst project made by me.

## Crime-Rate-USA
This dataset contains 1 million data points representing criminal incidents reported across the United States from January 2020 through March 2025.

### Dataset Highlights

Total Records: 1,000,000
Time Span: January 2020 – March 2025
Geographic Coverage: United States (nationwide, multi-state)
Data Format: CSV 

### Field                  Name                                        	Description	Type
incident_id	      Unique identifier for the crime event             	String
date	            Date and time of the incident                     	Datetime
state	            US state where the incident occurred	              String
city	            City or locality of the incident	                  String
latitude	        Latitude of the incident location	                  Float
longitude       	Longitude of the incident location	                Float
crime_type	      Type of crime (e.g., Assault, Theft, Robbery, etc.)	String
weapon_used	      Type of weapon used, if any	                        String
arrest_made	      Whether an arrest was made (Yes/No)	                Boolean
suspect_gender	   Gender of suspect (if known)                     	String
victim_gender   	Gender of victim (if known)                       	String
outcome	          Outcome (e.g., Arrested, Under Investigation, Unsolved)	String

### Steps:-
#### Data Processing & Cleaning
Before publishing the dataset, the following preprocessing steps were applied to ensure consistency, accuracy, and usability:

##### ✅ 1. Null Value Handling
Removed records with critical missing values such as:

incident_id

date

state or city

crime_type

For less critical fields (e.g., weapon_used, suspect_gender), missing values were:

Filled with 'Unknown' or 'Not Reported', depending on the context.

###### 📏 2. Outlier Detection & Removal
Applied statistical methods (e.g., IQR, Z-score) to detect and remove:

Implausible coordinates (e.g., outside US lat/lon bounds).

Invalid dates (e.g., future dates after March 2025).

Unrealistic values for numeric fields like weapon counts or arrests.

##### 🕒 3. Date & Time Normalization
Standardized all date fields to ISO 8601 format: YYYY-MM-DD HH:MM:SS.

Parsed and corrected malformed or inconsistent date entries.

Extracted additional temporal features:

year, month, day, weekday, and hour for time-based analysis.

## To demonstrate the value of this dataset, an interactive Power BI dashboard was created. The dashboard provides a visual exploration of crime trends across the United States from 2020 to March 2025.



