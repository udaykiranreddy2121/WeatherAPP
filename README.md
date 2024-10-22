Overview
This Weather Monitoring System fetches real-time weather data for multiple cities using the OpenWeatherMap API. The application collects data, processes it, stores daily summaries in a SQLite database, and visualizes temperature trends over time.

Features
Fetches weather data for multiple cities: Delhi, Mumbai, Chennai, Bangalore, Kolkata, and Hyderabad.
Stores daily weather summaries including average, maximum, and minimum temperatures.
Alerts the user if the temperature exceeds a specified threshold for consecutive readings.
Visualizes average temperature trends over time.
Dependencies
To set up and run this application, you'll need the following Python packages:

requests: For making HTTP requests to the OpenWeatherMap API.
pandas: For data manipulation and analysis.
SQLAlchemy: For database interactions and ORM functionality.
matplotlib: For data visualization.
Installation
You can install the required packages using the following command:

bash
Copy code
pip install requests pandas sqlalchemy matplotlib
Setup
Clone this repository to your local machine.
Install the required packages using the command above.
Replace the API_KEY in the code with your OpenWeatherMap API key.
Usage
Run the main.py file to start the weather monitoring system:
bash
Copy code
python main.py
The program will fetch the weather data every minute. After collecting sufficient data (for a full day), it will store the daily summaries in the SQLite database and visualize the average temperatures.

To stop the program, you can use CTRL + C.

Visualization
After running the program for a sufficient time (at least several iterations), the system will generate a graph showing the average temperature for each city over time.

Notes
Ensure that you have a stable internet connection as the application fetches data from an online API.
The application can be modified to adjust the threshold temperature for alerts or to add more cities.
The visualizations may require adequate data points, so it's recommended to run the application for at least 24 hours for the best results.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
OpenWeatherMap for providing the weather data API.
The Python community for its open-source libraries.
