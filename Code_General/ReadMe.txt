Service Transformer Primary Voltage Estimation Code

Input file:
Meter_XFMR_test.csv: Mapping file for AMI meter and transformer ID
AMI_V_test.csv: AMI voltage data
AMI_L_test.csv: AMI load data
XFMR_L_test.csv: Aggregated load data at service transformer
If the names of these files are changed, change the names line 36-46 in Main code 1 accordingly.

Main code 1:
This code read the AMI data and generate the machine learning model for each service transformer. 
Change the feeder’s name in line 30 when applying the code in another feeder.
Change line 49-55 when applying the code in another time duration.

Main code 2:
This code read the AMI data and machine learning model, then estimate the primary voltage for each service transformer.
Change the feeder’s name in line 29 when applying the code in another feeder.
Change line 47-53 when applying the code in another time duration.

Main code 3:
This code read the estimated voltage data and compare with Synergi power flow results (or actual voltages).
Change the feeder’s name in line 25 when applying the code in another feeder.
Change line 36-42 when applying the code in another time duration.
Change line 54 if using another error limit to determine buses with large errors.  
