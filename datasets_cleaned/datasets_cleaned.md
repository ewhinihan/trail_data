Datasets were cleaned using tidy data principles. Because of the nature of geospatial data, there were additional cleaning measures that were taken in some cases.
Outlined below are how each dataset was cleaned.

    File: Yakima_WA_TrailLines_2020_cleaned.csv
    Id column removed
    Type column removed
    "NA" added to cells with blank values
    Text in ROUTE TYPE column edited for consistency
    Activity tags broken out into 4 columns for bike, hike, horse, ski

    File: Seattle_WA_Traile_2021_cleaned.txt
    File saved as tab separated file to preserve special characters that were necessary for data interpretation as well as maintain dates in ISO 8601 format
    Shape_LENG, SHAPE_LE_1, GIS_LENGTH columns removed as the shape length was already represented in THE_GEOM field
    Column headers capitalized for consistency and expanded upon when attribute definition could be inferred (ex: GRADE_PERC renamed to GRADE_PERCENTAGE)
    "NA" added to cells with blank values or "-"
    "12:00:00 AM +0000" removed from DATE_TIME column and GIS_EDIT_DATE column and date formated to ISO 8601 date format standard
    
    
    File: 
