WeatherApp using Python with OpenWeatherAPI and requests library
This script uses the `requests` library to make an HTTP GET request to the OpenWeatherMap API. Here's a breakdown of the main components:

- `import requests`: This line imports the requests library, which is used to send HTTP requests easily.
- `api_key`: Your API key for the OpenWeatherMap API. You need to sign up on their website to get an API key.
- `user_input`: This variable prompts the user to input the city name.
- `weather_data = requests.get(...)`: This line sends a GET request to the OpenWeatherMap API, passing the city name, desired units (imperial in this case for Fahrenheit), and your API key as query parameters.
- `if weather_data.json()['cod'] == '404':`: Checks if the API response contains a '404' error code, which indicates that the city was not found.
- `weather = weather_data.json()['weather'][0]['main']`: Extracts the main weather condition from the API response.
- `temp = round(weather_data.json()['main']['temp'])`: Extracts and rounds the temperature from the API response.
- Finally, the script prints out the weather condition and temperature for the specified city.

This script demonstrates a simple usage of the `requests` library to interact with web APIs and retrieve data.
