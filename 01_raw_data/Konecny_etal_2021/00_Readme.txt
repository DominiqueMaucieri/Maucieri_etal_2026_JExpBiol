This ThermalManipulation_Data 00_readme.txt file was generated on 2021-05-25 by CASSANDRA KONECNY


GENERAL INFORMATION

1. Title of Dataset: ThermalManipulation_Data

2. Date of data collection : 
    Main text data: 2019-06-19
    Supplemental Data: 2021-03-20

3. Geographic location of data collection 

    Main article data: April Point, Quadra Island, British Columbia, Canada (50.064067, -125.236816)
    Supplemental Data: Spanish Banks beach, Vancouver, British Columbia, Canada (49.278124, -123.222027)

----------------------------------------------------------------------------------------------------------------
DATA & FILE OVERVIEW

1. File List: 

   Main text:
    - 01_Quadra_heatingData.csv: data was collected to evaluate the initial tidepool heating manipulation trial. 
                     The data contains information on abiotic parameters for each treatment 
                     condition.

    - 02_Quadra_coolingData.csv : data was collected to evaluate the tidepool cooling temperature manipulation 
                      trial. The data contains information on abiotic parameters for each treatment 
                      condition throughout the trial.


   Supporting Materials:
    - 03_SupplementalData_Trial1_HOBO.csv: data was collected to assess how pool temperatures and heating by the 
                       SAUTE may vary between containers of similar volume but different 
                       dimensions. This dataset provides high temporal resolution temperature 
                       measurements.

    - 04_SupplementalData_Trial1_SpotMeas.csv: data was collected to assess how pool temperatures and heating by the 
                           SAUTE may vary between containers of similar volume but different 
                           dimensions. This dataset contains spot measurements at a variety of 
                           locations (see diagrams in supplement of publication) throughout each 
                           container to better understand patterns of thermal variation within a 
                           container.
    - 05_SupplementalData_Trial2_HOBO.csv: data was collected to evaluate the ability of the SAUTE to heat a large
                       volume of water (100L). HOBO data loggers were placed at various 
                       locations (see diagrams in supplement of publication) throughout each 
                       container.
    - 06_SupplementalData_Trial2_SpotMeas: data was collected to evaluate the ability of the SAUTE to heat a large 
                       volume of water (100L). Spot measurements were taken at various 
                       locations (see diagrams in supplement of publication) throughout each 
                       container to assess thermal variation within a container. 

----------------------------------------------------------------------------------------------------------------
DATA-SPECIFIC INFORMATION FOR: [01_Quadra_heatingData.csv]

1. Number of variables: 8

2. Number of cases/rows: 135

3. Variable List: 
 - pool_ID: unique identifier for each pool
 - treatment: level of treatment condition (Ambient/Control/Heated)
 - time: time of measurement (PST, 24hr format)
 - temperature: water temperature (degrees celsius)
 - salinity: water salinity (psu)
 - pH: water pH
 - DO_mg_L : Dissolved Oxygen (mg/L) measured in a subset of pools and timepoints
 - DO_Percent : Dissolved Oxygen (%) measured in a subset of pools and timepoints

4. Missing Values: NA values indicate missing values. Data was not collected for given parameter(s) at these timepoints.

----------------------------------------------------------------------------------------------------------------
DATA-SPECIFIC INFORMATION FOR: [02_Quadra_coolingData.csv]

1. Number of variables: 5

2. Number of cases/rows: 64

3. Variable List: 
 - pool_ID: unique identifier for each pool
 - treatment: level of treatment condition (Cooled/Control)
 - time: time of measurement (PST, 24hr format)
 - temperature: water temperature (degrees celsius)
 - salinity: water salinity (psu)

----------------------------------------------------------------------------------------------------------------
DATA-SPECIFIC INFORMATION FOR: [03_SupplementalData_Trial1_HOBO.csv]

1. Number of variables: 5

2. Number of cases/rows: 1600

3. Variable List: 
 - Date-Time (PST): Date and time (PST & 24hr format) of temperature measurement
 - heating_treatment: level of treatment condition (Control/Heated)
 - container_type: type of experimental container used (bucket/tray)
 - container_ID: Identifier within each heating_treatment*container_type combination
 - temperature: water temperature (degrees celsius)

----------------------------------------------------------------------------------------------------------------
DATA-SPECIFIC INFORMATION FOR: [04_SupplementalData_Trial1_SpotMeas.csv]

1. Number of variables: 6

2. Number of cases/rows: 486

3. Variable List: 
 - container_type: type of experimental container used (bucket/tray)
 - container_ID: Identifier within each heating_treatment*container_type combination
 - heating_treatment:level of treatment condition (Control/Heated)
 - measurement_location:measurement locations within a container - corresponding diagram of locations in the 
   supplemental materials for the accompanying article (a,b,c,d,e)
 - time: time of measurement (PST, 24hr format)
 - temperature: water temperature (degrees celsius)
----------------------------------------------------------------------------------------------------------------
DATA-SPECIFIC INFORMATION FOR: [05_SupplementalData_Trial2_HOBO.csv]

1. Number of variables: 5

2. Number of cases/rows: 1190

3. Variable List: 
 - Date-Time (PST): Date and time (PST & 24hr format) of temperature measurement
 - heating_treatment: level of treatment condition (Control/Heated)
 - logger_depth: relative depth of data logger within each experimental container (shallow/bottom)
 - logger_location: relative logger location within each depth (corner/centre) * Note: Control treatment does not
   have data for the [shallow, corner] location *
 - temperature: water temperature (degrees celsius)

----------------------------------------------------------------------------------------------------------------
DATA-SPECIFIC INFORMATION FOR: [06_SupplementalData_Trial2_SpotMeas]

1. Number of variables: 6

2. Number of cases/rows: 20

3. Variable List: 
 - container_type: type of experimental container used (tub)
 - heating_treatment:level of treatment condition (Control/Heated)
 - measurement_location: measurement location within container based on cardinal directions (NE, NW, centre, SE,
   SW)
 - measurement_depth: relative depth of temperature measurement within each experimental container (shallow/
   bottom)
 - temperature: water temperature (degrees celsius)
 - time: time of measurement (PST, 24hr format)