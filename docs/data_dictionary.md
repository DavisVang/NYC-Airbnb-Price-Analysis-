# Data Dictionary

## Core Fields

| Field | Description |
|---|---|
| `Host_ID` | Unique identifier for the Airbnb host |
| `Host_Since` | Date the host joined Airbnb |
| `Listing_Name` | Listing title |
| `Neighbourhood` | NYC borough or neighborhood grouping used in the dataset |
| `Property_Type` | Type of property, such as apartment, house, loft, etc. |
| `Room_Type_Clean` | Cleaned room type category |
| `Zipcode` | ZIP code stored as text |
| `Beds` | Number of beds |
| `Number_Of_Reviews` | Count of listing reviews |
| `Price` | Listing price |
| `Review_Score` | Review score rating |

## Created Fields

| Field | Description |
|---|---|
| `Rating_Status` | Flags whether a listing has a rating or is missing a rating |
| `Review_Status` | Flags whether a listing has reviews or no reviews |
| `Review_Bucket` | Groups listings into No Reviews, Low Reviews, Medium Reviews, and High Reviews |
| `Price_Bucket` | Groups listings into Budget, Mid, Premium, and Luxury |
| `Price_Outlier_Flag` | Identifies high-price listings that may skew averages |
| `Data_Quality_Flag` | Flags rows requiring review |

## Analysis Notes

- `Zipcode` is stored as text because ZIP codes are labels, not quantities.
- Missing ratings were kept and flagged instead of deleted.
- Price buckets were used because average price can be skewed by expensive listings.
- Review buckets were used to compare listings by review activity.
