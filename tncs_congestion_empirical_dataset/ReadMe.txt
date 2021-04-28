Model estimation files for: 

    G.D. Erhardt, S. Roy, D. Cooper, B. Sana, M. Chen, J. Castiglione 
    "Do Transportation Network Companies Decrease or Increase Congestion?" (2018)

Please feel to email greg.erhardt@uky.edu to obtain more information about this dataset.


There are two files in the same format: 

    ESTFILE_2010.csv - reflecting year 2010 conditions
    ESTFILE_2016.csv - reflecting year 2016 conditions
    
Each file has one record for each ModifiedTMC and TOD, with the records matched between the two years.  
The columns are as follows:

ID - a unique ID, which is a combination of the next two fields
ModifiedTMC	- ID for the spatial unit of analysis, a directional section of roadway
TOD	- Time-of-day: AM=6-9 AM, MD=9 AM-3:30 PM, PM=3:30-6:30 PM, EV=6:30 PM-3:00 AM, EA=3-6 AM
YEAR - The year, either 2010 or 2016
CHAMP_LINK_COUNT - The number of SF-CHAMP links that aggregate to this ModifiedTMC
PRESIDIO - Binary flag indicating whether the ModifiedTMC is on the Presidio Parkway or Veterans Blvd
PHF	- Peak Hour Factor, the share of the total period volume that occurs in the highest 1-hour period
ALPHA - alpha term for use in VDF
BETA - beta term for use in VDF
AT - Area Type: 0=Regional Core, 1=Central Business Distritc, 2=Urban Business, 3=Urban
FT2 - Facility Type: 1-Freeway, Expressway or Ramp, 2=Major Arterial, 3=Minor Arterial, 4=Local or Collector
LANES - Number of lanes (can be non-integer due to averaging across SF-CHAMP links)
DISTANCE - distance in miles
CAPACITY - capacity in vehicles for the period as a whole
FFS	- free flow speed
INRIX_SPEED	- average speed, as measured by INRIX data
SPEED_20TH - 20th percentile speed, as measured by INRIX data
FF_TIME	- free flow travel time
INRIX_TIME - average travel time, as measured by INRIX data
INRIX_VOL - implied volume
CHAMP_PCE - SF-CHAMP passenger car equivalents (PCEs)
CHAMP_VOL - SF-CHAMP volume (vehicles)
TNC_VOL	- TNC volume
TNC_PUDO - TNC pick-ups and drop-offs
AVG_DUR	- TNC average duration variable, calculated as: (CAPACITY/LANES) * (TNC_PUDO / (3600/PHF]))
AVG_DUR_MAJOR_ARTERIALS	- TNC average duration variable on major arterials, zero elsewhere
AVG_DUR_MINOR_ARTERIALS	- TNC average duration variable on minor arterials, zero elsewhere
BASE_INRIX_VOL_PRESIDIO - In 2016, the base year (2010) implied volume on the Presidio Parkway or Veterans Blvd, zero elsewhere.  In 2010, zero everywhere. 
