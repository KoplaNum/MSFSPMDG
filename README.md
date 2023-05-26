MSFS to PMDG Flight Plan Converter
This Python script converts Microsoft Flight Simulator (MSFS) flight plan files (.pln) into PMDG .rte flight plan files.

Features
The script parses an MSFS flight plan file, extracting waypoint data and converting coordinates from degrees/minutes/seconds (DMS) to decimal format.

It then generates a PMDG-compatible flight plan, assigning a type to each waypoint (1 for departure and arrival airports, 5 for other waypoints), and writing data to the output file in the correct format.

Waypoints classified as 'SIDSTARAPP' in the MSFS file are excluded from the converted flight plan.

Usage
To use the script, you need to pass the input (.pln) file and output (.rte) file as arguments:

CMD prompt :

python convert_flightplan.py input.pln output.rte

Upon successful conversion, a message indicating the completion will be displayed.

Requirements
This script requires Python 3 and the xml.etree.ElementTree module for XML parsing.

Note
Always ensure you have backups of your flight plan files before conversion, as the operation modifies the files and is not reversible.

Author
KoplaNum

License
[License]
