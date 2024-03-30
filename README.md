<h1> Weather App with Python using OpenWeather API and requests library </h1> <br/>
1 - First of all you need to install the requests library if you haven't already. You can install it using pip, which typically comes bundled with Python.<br/>
<i>"pip install requests"</i> <br/>
2 - Then import it into your project.  <br/>
<i>"import requests"</i> <br/>
The requests library in Python is used for making HTTP requests and handling responses in a simple way. <br/>
This library provides an easy-to-use interface for accessing resources (URLs) on the web. <br/>
It's commonly used for scenarios such as interacting with web APIs, downloading web pages, or fetching web-based content. <br/>
Some of its functionalities include: <br/>
Sending HTTP requests and receiving responses (using methods like GET, POST, PUT, DELETE, etc.).<br/>
Managing URL parameters, headers, cookies.<br/>
Uploading and downloading files.<br/>
Security measures: SSL certificate verification, session management, user authentication, etc.<br/>
Handling various data formats such as JSON, XML, etc.<br/>
3 - <i>"api_key ='...' "</i> <br/>
Log in/sign up to your OpenWeatherMap account and copy your API Key. <br/>
4 - <i>"user_input = input("Enter city: ")"</i> <br/>
It creates an input field asking the user to enter a city name. <br/>
5 - <i>"weather = weather_data.json()['weather'][0]['main']"</i> <br/>
This line extracts the main weather condition for the specified city from the JSON response obtained from the API. It accesses the first element of the 'weather' list within the JSON response and then extracts the 'main' key, which represents the main weather condition (e.g., 'Clear', 'Clouds', 'Rain', etc.).<br/>
6 - <i>"temp = round(weather_data.json()['main']['temp'])"</i> <br/>
Here, the temperature for the specified city is extracted from the JSON response. It accesses the 'temp' key under the 'main' object in the JSON response, which represents the current temperature. The temperature is rounded to the nearest integer using the round() function.<br/>
7 - Finally print the info in the way you want.

