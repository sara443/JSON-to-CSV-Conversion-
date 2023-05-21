# JSON-to-CSV-Conversion


JSON-to-CSV Conversion Objective: 


The goal is to create a Python script that can convert JSON files into CSV format. The script reads JSON files from a specified source directory, extracts relevant information, and saves it as CSV files in a designated target directory.
Conversion Process: 

The script performs the following transformations on the data:

1.	Extracts only the necessary columns from the input JSON files.
2.	Renames the columns to enhance readability.
3.	Splits the user_agent column into web_browser and operating_sys columns.
4.	Extracts the operating system from the operating_sys column.
5.	Extracts the domain from the from_url and to_url columns.
6.	Splits the longitude_latitude column into latitude and longitude columns.
7.	Rounds the latitude and longitude columns to 2 decimal places.
8.	Removes any rows with missing data in the city, longitude, or latitude columns.
Getting Started:

To use this script, follow these steps:
1.	Install Python 3 on your computer if you haven't already.
2.	Download the script file named "json_csv_convertor.py" from the repository and save it to your desired location.
3.	Open a terminal or command prompt and navigate to the directory where the script is located.
Running the Script: 

Execute the script using the following command: python json_csv_convertor.py <source_dir> <target_dir> <unix_time>
•	<source_dir>: The path to the directory containing the JSON files you want to convert.
•	<target_dir>: The path to the directory where you want to save the resulting CSV files (optional - if not provided, the CSV files will be saved to the source directory).
•	<unix_time>: An optional flag that specifies whether to output time in Unix format or human-readable format (default is human-readable format).
Example Usage: 

python json_csv_convertor.py /path/to/json/files /path/to/csv/files yes This example command will convert all JSON files in the /path/to/json/files directory to CSV files and save them in the /path/to/csv/files directory, including timestamps in Unix format.
Dependencies: 

The script requires the following Python packages to be installed:
•	pandas
•	numpy
You can install these packages using pip: pip install pandas numpy
