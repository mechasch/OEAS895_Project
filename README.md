# OEAS895_Project

This data repository contains code for an ocean data course (OEAS895) at Old Dominion University. The project utilizes a supervised machine learning algorithm to predict summer dissolved inorganic nitrogen (DIN) concentrations in the Chesapeake Bay estuary, particularly in the Lafayette River sub-tributary. 
All files necessary to run the code in this repository is included within.
The repository contains the following contents:

1. Combined_List_R_UPDATED_HEADERS.csv - This .csv file contains all the combined data for this project; nitrogen samples, YSI 6600 V2 sonde measurements, wind speed/direction data, daily precipitation totals, and tidal height. NaN values are included for no probe or verified poor values. The detection limit for DIN is 0.14 uM and is displayed as such in the file. The units for these variables are as follows:
		
		* Date: M/D/YYYY
		* Month: M
		* Day: D
		* Year: YYYY
		* Depth_ID: INT
		* Depth: meters
		* Time: hh:mm
		* NH4: uM
		* UREA: uM
		* DIN: uM
		* PO4: uM
		* Temp: degrees Celcius
		* Sal: no units
		* pH: no units
		* Chl: ug/L
		* Turb: NTU
		* DO: mg/L
		* Tide: meters MSL
		* Precipitation: meters
		* Wind_Speed: meters/second
		* Wind_Dir: 0-360 degrees
		* Bloom: Boolean
		
2. Project_Exloratory_Analysis_Final.ipynb - this is an exploratory analysis of the target variable (DIN) and the predictor variables. Data distributions and DIN vs. predictor relationships are explored among different depths and years. A seasonality of sample amounts is also available for each year.

3. Model_BOTH_DEPTH_041720.ipynb - Data is randomized and separated into depth id's of 1 and 3 only from June-September. A random forest regression model is then built using measured DIN concentrations, climatological data, and water quality parameters all measured in the Elizabeth and Lafayette River watersheds. 

4. Model_D1_041720.ipynb - Data is randomized and separated by a depth id of 1 only from June-September. A random forest regression model is then built using measured DIN concentrations, climatological data, and water quality parameters all measured in the Elizabeth and Lafayette River watersheds.

5. Model_D3_041720.ipynb - Data is randomized and separated by a depth id of 3 only from June-September. A random forest regression model is then built using measured DIN concentrations, climatological data, and water quality parameters all measured in the Elizabeth and Lafayette River watersheds.

Future use: The plan for this model is to be used alongside moored YSI sondes at the Norfolk Yacht and Country Club (NYCC), Ashland Circle (AC), tidal height data, and climatological data to determine DIN concentrations when we are not sampling in the field. Theoretically, this model will be very useful for DIN in the summer months, but could eventually be expanded to cover each season.

This model is unique to the Chesapeake Bay estuary and should be used with caution on other systems.

Tidal data available: https://tidesandcurrents.noaa.gov/stationhome.html?id=8638610

Wind and precipitation data available at: https://www.ncdc.noaa.gov/cdo-web/datasets/LCD/stations/WBAN:13737/detail

For questions, please email Michael Echevarria @ meche002@odu.edu

