# Vehicle Simulation Project

## Overview
This project simulates the movement of a vehicle, including:
- Speed fluctuations based on acceleration and deceleration.
- Directional changes in movement.
- GPS location updates to reflect motion.
- Real-time weather data retrieval from OpenWeather API.

## Features
- **Dynamic Speed Simulation:** Accelerates and decelerates randomly within defined limits.
- **Location Tracking:** Updates latitude and longitude based on speed and direction.
- **Weather Integration:** Fetches real-time weather data at the vehicle's simulated GPS location.
- **Customizable Vehicle Properties:** Includes parameters such as fuel type, brand, and engine type.

## Requirements
Before running the project, ensure you have the following installed:
- Python 3.x (You can suit things that is best to you. Is not really a dealbreaker requirement tho.)
- `requests` package (for fetching weather data)

## Installation
1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```

2. Install the required dependencies:

    If you dont have virtualenv dont do it. When you use:

    ```bash
    pip freeze > requirements.txt
    ```

    This command that is right above it. Its gonna import all of the current used pip packages. :( Well you can import them yourselves as well.

   ```bash
   pip install -r requirements.txt
   ```

## Configuration

First 1000 API calls per day are free. You can comment them out. Its gonna be in Istanbul anyway.(So the weather itself not gonna change that much within same city...)

Modify the script to set up API keys and relevant parameters:

- OpenWeather API key (OpenWeather_API_KEY in the script)

- Initial coordinates (start_location)

## Usage

Run the simulation using:

   ```bash
   python simulate_vehicle.py
   ```
- The script will continuously simulate vehicle motion until manually interrupted.
- Speed, GPS, and weather data will be displayed in the terminal.

### Example Output

   ```bash
Vehicle Data: {'deviceId': '06ebc819-e060-47d7-97cb-5d51a65c0f19', 'timestamp': '03:16:17', 'direction': ['W', 'N'], 'speed': -0.7120458046716643, 'fuelType': 'Hybrid', 'brand': 'Audi', 'model': 'RS7', 'engineType': 'V8'}
GPS Data: {'deviceId': '06ebc819-e060-47d7-97cb-5d51a65c0f19', 'timestamp': '03:16:17', 'latitude': 41.0082, 'longitude': 28.97839861625027}
Weather Data: {'timestamp': '03:16:17', 'temperature': 9.980000000000018, 'humidity': 34, 'wind_speed': 2.57}
   ```
   
   You can always comment out weather data stuff. And generate yourself your own data for playing around with it.
   
 ### Notes

- The maximum speed is capped at 250 km/h for simulation purposes. (My car choice specs.)

- The simulation runs indefinitely until manually stopped (CTRL + C) in terminal if you are using .py file. Rip to .ipynb users..

- Weather data updates dynamically based on the simulated vehicle's GPS location.

### Contributors

    Contributions are always welcomed. Feel free to hit me up with the requests and contribute also you can report an issue as well