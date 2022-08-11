# TracksMining
This contains the TracksMining code, intended to explore animal telemetry data

# How to run the application

# STEP 1 : DOWNLOAD TracksMining.zip

Once uncompressed, this folder contains 4 subfolders:
"data" : This folder host data essential to TracksMining
"output" : This is the folder where outputs will be recorded
"scripts" : This folder host the scripts of the application
"settings" : This folder host the settings (provided as an less-convenient alternative to the user interface)

At startup, the "output" folder is empty.

The "data" folder contains 4 subfolders:
"interaction" : The interaction files (.geojson) must be stored in here
"positions" : GPS files (.csv or .txt) must be stored in here.
"templates": Contains the templates for the interactive map
"templates_html": Contains the templates for the interface.  Is is recommanded not to modify them.

The "scripts" folder contains 3 files:
- TracksMining.py : Is a Python file holding the controller and all classes.
- TracksMining_localserver.py : Is a Python file running a flask application to run the user interface.

It is important to keep this structure and names of folders.

# STEP 2 : CHECK IF DEPENDENCIES ARE INSTALLED ON YOUR COMPUTER
TracksMining requires many external dependencies:
Folium, MatPlotLib, Pandas, Numpy, Shapely, PyTZ, ScikitLearn, etc.
Flask is required for local server utilization.
Make sure these dependencies are installed on your local disk.


# STEP 3A : EXECUTE WITH A LOCAL SERVER INTERFACE

Open TracksMining_localserver.py and run the file.
Click on the link displayed in the console to access the user interface.


# STEP 3B : EXECUTE WITH A EXCEL SETTING INTERFACE (Alternative to local Server Interface)

In "settings", open "settings.xls" and play with parameters.
SAVE THE FILE TO UPDATE SETTINGS
Open TracksMining.py and run the file.
Check in the output folder for the new folder.

Note: As all folders are kept in output, empty this folder on a regular basis.
