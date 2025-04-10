## 🌦️ Weather API Automation
This is a simple Python script that interacts with the OpenWeatherMap API to fetch and display real-time weather information for a city provided by the user. The script retrieves full weather data in JSON format and then extracts key information such as weather description, temperature, sunrise, and sunset times.

## 📁 Project Structure
* WeatherAPIautomation.ipynb: Main notebook that contains the code to make API requests and display the weather.
* .env: A hidden file that securely stores your API key.

## 🔧 Requirements
Make sure you have the following Python libraries installed:
```
  pip install requests python-dotenv]
```

## 🔐 Setting Up API Key
1. Create a free account at OpenWeatherMap.
2. Navigate to your dashboard and copy the API key.
3. Create a .env file in your working directory and add the following:
   ```
    key=YOUR_API_KEY_HERE
   ```

## ▶️ How to Run
1. Run the script or notebook.
2. Enter the name of the city when prompted.
3. The script will first print the full JSON data (for debugging or inspection).
4. Then it will ask again for a city and show a clean weather summary:
* Weather description
* Temperature (in Celsius)
* Sunrise and Sunset times (adjusted for timezone)

## 📝 Sample Output
Welcome to our weather reporter! Select a city to view?
Enter a City Name: London
Weather Summary:  broken clouds
Temperature is:  18.67 Celsius
Sunrise at:  2025-04-10 05:45:23
Sunset at:  2025-04-10 18:34:50

## ⚠️ Notes
* The temperature returned by OpenWeatherMap is in Kelvin, which is converted to Celsius in the script.
* Sunrise and sunset times are converted to local time using the timezone offset provided in the response.

## 📌 To-Do / Improvements
* Add error handling for invalid city names.
* Implement retries for failed requests.
* Convert to a fully interactive CLI or GUI application.
* Support batch weather checks for multiple cities.

## 📄 License
This project is open-source and free to use under the MIT License.
