Sensor Data Logger - README
Overview
This Python script functions as a Sensor Data Logger specifically designed for the DHT11 sensor. The script captures temperature and humidity data from the sensor and records it into an MYSQL database. The logged data is stored in a table named DHT_data. The script has a sample frequency set to 5 seconds, indicating that data is sampled from the sensor every 5 seconds.

Requirements
Adafruit_DHT Library
Ensure the Adafruit_DHT Python library is installed before running the script. Install it using:

bash
Copy code
pip install Adafruit_DHT
Library information: Adafruit CircuitPython DHT

MYSQL Module
The script uses the built-in MYSQL module in Python for database interactions. No separate installation is required.

Usage
Install Required Libraries:

Use the provided pip command to install the Adafruit_DHT library.
Hardware Setup:

Connect the DHT11 sensor to the appropriate GPIO pins on your hardware.
Run the Script:

Execute the Python script on your device.
bash
Copy code
python sensor_data_logger.py
Monitor Data:
The script will begin logging temperature and humidity data into the MYSQL database.
Database Structure
The script creates an MYSQL database with the following structure:

Database Name: sensor_data.db
Table Name: DHT_data
Columns:
timestamp: Time of data logging
temperature: Recorded temperature
humidity: Recorded humidity
Notes
Adjust GPIO pin configuration in the script based on your hardware setup.
Ensure proper permissions for accessing GPIO pins on your device.
Customize the script for different sensor models or database requirements
