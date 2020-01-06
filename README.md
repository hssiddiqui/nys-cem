# The New York State - Clean Energy Model (NYS-CEM)


## Data and Results

Data and results for the study 'Prioritizing heating and transport electrification to implement New York’s new climate law' (under review) are available in the linked Google [storage bucket](https://console.cloud.google.com/storage/browser/nys-cem_data_and_results?project=nys-cem&authuser=1&supportedpurview=project). 

## File Overview

`main.py`: The script used to run the NYS-CEM. This file loads the desired NYS-CEM model and the parameters given in `params.yaml`; it then specifies the amount of the low-carbon electricity to be supplied, the electrified heating load, and the electrified transport load; finally, it runs the model and calls the results processing functions given in `utils.py`.

`model_dual_trans_constrs.py`: The file used to create a version of the NYS-CEM that uses dual transmission constraints to govern interregional transmission. 

`model_dual_trans_vars.py`: The file used to create a version of the NYS-CEM that uses dual transmission variables to govern interregional transmission. 

`params.yaml`: The file that holds the NYS-CEM and Gurobi solver parameters.

`utils.py`: The file that contains multiple helper functions, including those that load the model parameters, the time-series data, and process the results.  
