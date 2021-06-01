Datasets were cleaned using tidy data principles. Because of the nature of geospatial data, there were additional cleaning measures that were taken in some cases.
Outlined below are details of how each dataset was normalized. All cleaned datasets are in open, non-proprietary formats to facilitate reuse by potential users
of the Repository. Limitation of these datasets include varying attributes for each dataset, inconsistent measurement units across similar attributes, and each
dataset had various ways of indicating location of trails.

    File: Yakima_WA_TrailLines_2020_cleaned.csv
    Id column removed
    Type column removed
    "NA" added to cells with blank values
    Text in ROUTE TYPE column edited for consistency
    Activity tags broken out into 4 columns for bike, hike, horse, ski

    Files: Seattle_WA_Trails_2021_cleaned.txt | Seattle_WA_Trails_2021_cleaned.csv
    File saved as tab separated file in addition to .csv format to preserve special characters that were necessary for data interpretation as well as maintain dates 
    in ISO 8601 format
    Shape_LENG, SHAPE_LE_1, GIS_LENGTH columns removed as the shape length was already represented in THE_GEOM field
    Column headers capitalized for consistency and expanded upon when attribute definition could be inferred (ex: GRADE_PERC renamed to GRADE_PERCENTAGE)
    "NA" added to cells with blank values or "-"
    "12:00:00 AM +0000" removed from DATE_TIME column and GIS_EDIT_DATE column and date formated to ISO 8601 date format standard
    Width column removed because it did not indicate measurement unit, which is a requirement for this attribute.
    
    File: WA_NationalForestSystemTrails_2021_cleaned.txt | WA_NationalForestSystemTrails_2021_cleaned.csv
    File saved as tab separated file in addition to .csv format to preserve special characters that were necessary for data interpretation as well as maintain dates 
    in ISO 8601 format
    ADMIN_ORG column removed as it had the same values as MANAGING_ORG column
    EMP column removed as it had duplicate values to SEGMENT_LENGTH
    ATTRIBUTESUBSET column removed as it did not add value to the dataset and was an administrative value
    All blank cells replaced with "NA" and "N/A" replaced with "NA" for consistency
    Formatted columns GIS_MILES, TRAIL_CN, SEGMENT_LENGTH to have consistent number of decimal places
    Removed WATER_MOTORIZED column as it only contained null values
    Removed NONMOTOR_WATERCRAFT_ACCPT_DISC column as it only contained null values
    Removed NONMOTOR_WATERCRAFT_MANAGED column as it only contained null values
    Removed MOTOR_WATERCRAFT_ACCPT_DISC column as it only contained null values
    Removed MOTOR_WATERCRAFT_MANAGED column as it only contained null values
    Renamed values in TRAIL_SURFACE for consistency (ex: replaced AC-ASPHALT with ASPHALT)
    Removed special characters, including "%" and replaced with decimals
    
    File: WA_RCOTrails_2017_cleaned.txt | WA_RCOTrails_2017_cleaned.csv
    File saved as tab separated file in addition to .csv format to preserve special characters that were necessary for data interpretation as well as maintain dates 
    in ISO 8601 format
    Replaced blank spaces with "NA" to represent null values
    Removed created_user and last_edited_user columns as they contained a user name that was not relevant to the data
    Removed NOT_SPECIFIED column as it only had null values
    Removed REVIEW_FLAG column as it only contained "yes" value which corresponds to REVIEW_COMMENTS column
    Normalized the created_date and last_edited_date columns to standardize date to ISO 8601 format (removed timestamp)
    Normalized TR_LENGTH column to make decimal places consistent
    
    
    
    
