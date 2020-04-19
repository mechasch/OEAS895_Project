# OEAS895_Project

This data repository contains code for an ocean data course (OEAS895) at Old Dominion University. The project utilizes a supervised machine learning algorithm to predict summer dissolved inorganic nitrogen (DIN) concentrations in the Chesapeake Bay estuary, particularly in the Lafayette River sub-tributary. 
All files necessary to run the code in this repository is included within.
The repository contains the following contents:

1. Combined_List_R_UPDATED_HEADERS.csv - This .csv file contains all of the combined data for this project; nitrogen samples, YSI 6600 V2 sonde measurements, wind speed/direction data, daily precipitation totals, and tidal height. The units for these variables are as follows:
		
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
2. Project_Exloratory_Analysis_Final.ipynb - 
3. Model_BOTH_DEPTH_041720.ipynb -
4. Model_D1_041720.ipynb -
5. Model_D3_041720.ipynb -
