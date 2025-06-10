# Weather Dashboard
![image](https://github.com/user-attachments/assets/d44921b3-defc-44dd-9c5d-b9d30207b21b)
## Key Features
- Template nodes with CSS. The design of the widgets resemble that of smart watches. The color palette is based on the color scheme of the [icons](https://openweathermap.org/weather-conditions) made available by OpenWeatherMap.
- Function nodes for timestamp conversion, dynamic images (i.e. section of `img` link changes based on the weather), case conversion (i.e. lowercase to Title Case), and wind direction calculations.

> [!WARNING]
> Free OpenWeatherMap API keys have a limited number of 60 calls per minute. Hourly forecast and daily forecast are unavailable.

> [!TIP]
> During the development phase, consider manual reinjection as opposed to reinjection at intervals.

## Running the Dashboard Locally

### Node.js
1. Install the latest LTS version of [Node.js](https://nodejs.org/en/).

### Node-RED
2. In command prompt, execute `npm install -g --unsafe-perm node-red`.
> [!NOTE]
> `-g` installs Node-RED as a global module.
3. Execute `node-red`.
4. Locate the link preceded by a timestamp followed by [info] Server now running at. Click on the link to access the Node-RED development environment and runtime dashboard in your web browser.
> [!CAUTION]
> Terminal must be kept open to keep Node-RED running.

### OpenWeatherMap
5. Create an account in [OpenWeatherMap](https://openweathermap.org/). Confirm your email.
6. Click on your username > My API keys. Copy the available API key or generate then copy a new one.

### Development Environment 
7. 

## Replication

- References:
  - [Running on Windows: Node-RED](https://nodered.org/docs/getting-started/windows)

- Font: DotGothic16 [Google Fonts](https://fonts.google.com/specimen/DotGothic16/) [GitHub](https://github.com/fontworks-fonts/DotGothic16)
- Icons: https://openweathermap.org/weather-conditions

