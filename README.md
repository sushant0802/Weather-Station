# Mini_Weather_Station ✨
Making a mini weather station that runs on [ **ESP8266,( WeMos D1 Mini )**].
<p align="center">
  <kbd>
<img src="https://user-images.githubusercontent.com/97898007/189523499-2e932f05-3a5e-427e-bb07-b9bc0dd26f52.gif"></img>
  </kbd>
</p>
This project is the production of a mini size weather station of about 45mm x 45mm x 50mm using [WeMos D1 Mini (ESP8266)].
I am using the OpenWeather API to get weather data.
It also measures indoor real-time temperature and humidity using DHT22 (or DHT11).
- I am attaching the Arduino code. (including 2 header files)
[WeatherStation.ino/WeatherStationFonts.h/WeatherStationImages.h]

Please modify the Wi-Fi SSID & password, time zone, OpenWeather API key, and location ID items according to your environment!

# Install and configure Arduino IDE
 Make sure you use a version of the Arduino IDE which is supported by the ESP8266 platform.
 [(https://www.arduino.cc/en/software)]

# Install libraries in Arduino IDE
 First, install the required libraries.There are several. `Go to Sketch` > `Include Libraries` > `Manage Libraries`, search for the "mentioned libraries" and click Install. Take a break until the installer finishes.
![Screenshot 2022-08-12 005333](https://user-images.githubusercontent.com/97898007/184223658-1f6d62a2-21fa-4493-a234-f824e67d37c8.jpg)
 - [Json Streaming Parser]
 - [ESP8266 and ESP32 OLED driver for SSD1306 displays]
 - [ESP8266 Weather Station]
 - [DHT sensor library for ESPx]

# Used parts list:
![Screenshot 2022-08-12 004242](https://user-images.githubusercontent.com/97898007/184220664-9383d416-03b1-4534-b1e8-8b41934f35e8.jpg)
 - WeMos D1 Mini (Lolin)
 - OLED display (0.96 inch)
 - Temperature and humidity sensor DHT22 (or DHT11)
 - Charging module TP4056
 - Lipo battery (about 150mAh)
 - Power switch
 - M2 x 6mm tapping screws (14)
 
## Modify sketch:
 - Wi-Fi settings
 - Setting the time zone
 - Setting the update interval
 - DHT22 or DHT11 settings
 - OLED display I2C address
 - Setting the OpenWeather API Key
 - Setting the location ID
 - Writing a sketch, connection
 - Incorporation into the case
 
 ## Setting the OpenWeather API Key
This sketch uses the OpenWeather API to obtain weather data from various places from the internet via Wi-Fi.

OpenWeather is a service that can acquire weather data such as temperature, probability of precipitation, humidity and atmospheric pressure all over the world.
I will omit the details, but it is necessary to issue an API key to obtain these weather data . **(User registration is required!)**
You can get a lot of data with the paid version, but there is no particular problem with the free version for the mini weather station I made this time!

Issuing an API key is easy!. 
First, register as an OpenWeather user.[(https://openweathermap.org/)] (Email address and password setting only) .

![Screenshot 2022-08-12 013302](https://user-images.githubusercontent.com/97898007/184230281-c3fac93e-5d57-41b6-b984-1bf25c6b8734.jpg)

After completing user registration, log in to the site and go to the [ My API Keys ] page to display your API key.

**That's all! :+1:**
