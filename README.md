# Chicago Crime

Notice: The analysis conducted does not represent an official analysis.

This dataset reflects reported incidents of crime (with the exception of murders where data exists for each victim) that occurred in the City of Chicago from 2020 to present, minus the most recent seven days. Data is extracted from the Chicago Police Department's CLEAR (Citizen Law Enforcement Analysis and Reporting) system. In order to protect the privacy of crime victims, addresses are shown at the block level only and specific locations are not identified.

### Datasource:
https://catalog.data.gov/dataset/crimes-2001-to-present?from_hint=eyJzb3J0IjoicG9wdWxhcml0eSJ9 \
https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/about_data \
Support: https://datahub.cmap.illinois.gov/maps/CMAPGIS::community-data-snapshots-historical-data-2015-2026/about

### Dataset Period:
23 Jan 2020 - 05 Oct 2026

### Variables:
| Variable | Descriptions |
| --- | --- |
| `ID` | Unique identifier for the record. |
| `Case Number` | The Chicago Police Department RD Number (Records Division Number), which is unique to the incident. | 
| `Date` | Date when the incident occurred. this is sometimes a best estimate. | 
| `Block` | The partially redacted address where the incident occurred, placing it on the same block as the actual address. | 
| `IUCR` | The Illinois Uniform Crime Reporting code. This is directly linked to the Primary Type and Description. | 
| `Primary Type` | The primary description of the IUCR code. | 
| `Description` | The secondary description of the IUCR code, a subcategory of the primary description. | 
| `Location Description` | Description of the location where the incident occurred. | 
| `Arrest` | Indicates whether an arrest was made. | 
| `Domestic` | Indicates whether the incident was domestic-related as defined by the Illinois Domestic Violence Act. | 
| `Beat` | Indicates the beat where the incident occurred. A beat is the smallest police geographic area – each beat has a dedicated police beat car. Three to five beats make up a police sector, and three sectors make up a police district. The Chicago Police Department has 22 police districts. | 
| `District` | Indicates the police district where the incident occurred. | 
| `Ward` | The ward (City Council district) where the incident occurred. | 
| `Community Area` | Indicates the community area where the incident occurred. | 
| `FBI Code` | Indicates the crime classification as outlined in the FBI's National Incident-Based Reporting System (NIBRS). | 
| `X Coordinate` | The x coordinate of the location where the incident occurred in State Plane Illinois East NAD 1983 projection. This location is shifted from the actual location for partial redaction but falls on the same block. | 
| `Y Coordinate` | The y coordinate of the location where the incident occurred in State Plane Illinois East NAD 1983 projection. This location is shifted from the actual location for partial redaction but falls on the same block. | 
| `Year` | Year the incident occurred. | 
| `Updated On` | Date and time the record was last updated. | 
| `Latitude` | The latitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block. | 
| `Longitude` | The longitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block. | 
| `Location` | The location where the incident occurred in a format that allows for creation of maps and other geographic operations on this data portal. This location is shifted from the actual location for partial redaction but falls on the same block. | 

### Exploratory Data Analysis:
* Handling duplicates 
* Handling missing values
* Removing outliers
* Data visualizations

### Conclusions:
Determine cluster/wards based on historical crimes data, and find the center of each cluster by using Unsupervised Machine Learning approach. By doing so, it is hoped that crimes can be mitigated around the clustered area.\
<img width="1217" height="685" alt="Chicago Crimes" src="https://github.com/user-attachments/assets/e2565b52-f417-4130-88f2-0f109a53e0da" />



