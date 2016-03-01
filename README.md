## exc_to_pt.py

###ArcPy

###Description: Python script that utilizes arcpy to create a project file gdb, loop through all project .xlsx files and sheets (tables) in the given path, and convert all relevant tables to feature classes in the new project gdb. This script is used for the preparation of Texas crash and/or citation data for use in Texas DPS-HSOC geospatial products.

###Preparation:
1. Only tables (sheets) with both "Lat" and "Lon" field names can be included, otherwise the program will print an error.
2. Insure there are no spaces or strange characters in the sheet names of each excel file. Give each sheet a descriptive name such as "Crash_2015".

###Instructions to run program:
1. Open a command window in the same directory that this script is saved - hold shift and right-click anywhere in the directory, choose 'open command window here'.
2. Type 'python exc_to_pt.py' and Press Enter. - this only works if you have already added python to the path in the system environment variables (Windows). If you have not done this, you will need to do so or use an IDE to run this script, such as IDLE or PyCharm, etc.
3. When prompted, enter the path to where your project xlsx files are saved. Press Enter.
4. When prompted, enter the name of your project file geodatabase, including the .gdb file extension. Press Enter.
5. If the program is running and completes successfully, you should see several print statements as the program is running, and then a print statement that reads 'PROGRAM COMPLETED SUCCESSFULLY'. Navigate to your project path and view the gdb and featureclasses to make sure everything is good to go. !Viola!
