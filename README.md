# Weather Dashboard
<img width="1920" height="827" alt="image" src="https://github.com/user-attachments/assets/d2720b89-f2ba-4983-b38f-6682fbd4ecb4" />
<img width="1920" height="827" alt="image" src="https://github.com/user-attachments/assets/420e5930-a9db-4957-8853-303e3f7af8f0" />

## Key Features
- Template nodes with CSS. The design of the widgets resembles that of smart watches. The color palette is based on the color scheme of the [icons](https://openweathermap.org/weather-conditions) made available by OpenWeatherMap.
- Function nodes for timestamp conversion, dynamic images (i.e. section of `img` link changes based on the weather), case conversion (i.e. lowercase to Title Case), and wind direction calculations.

> [!WARNING]
> Free OpenWeatherMap API keys have a limited number of 60 calls per minute. Hourly forecast and daily forecast are unavailable.

> [!TIP]
> During the development phase, consider manual reinjection as opposed to reinjection at intervals.

## Running the Dashboard Locally

### Node.js
1. Install the latest LTS version of [Node.js](https://nodejs.org/en/).

### Node-RED
2. In the command prompt, execute the following:
   
   ```
   npm install -g --unsafe-perm node-red
   ```
> [!TIP]
> To open the command prompt using keyboard shortcuts, simply press <kbd>Win + R</kbd> then type `cmd`.

> [!NOTE]
> `-g` installs Node-RED as a global module.
3. Start the Node-RED server.

   ```
   node-red
   ```
4. Locate the link preceded by a timestamp followed by `[info] Server now running at`.
5. <kbd>Ctrl + click</kbd> on the link to access the Node-RED workspace and runtime dashboard in your web browser.
> [!CAUTION]
> Terminal must be kept open to keep Node-RED running.

### OpenWeatherMap
6. Create an account in [OpenWeatherMap](https://openweathermap.org/). Confirm your email.
7. Click on your username > My API keys. Copy the available API key or generate then copy a new one.

### Workspace 
8. Download the [flows.json](https://github.com/ABagram/node-red-weather-dashboard/blob/main/flows.json) file.
9. <kbd>Ctrl + I</kbd> to open the `Import nodes` overlay. 
10. Click on `select a file to import`. This will open the file dialog box. Locate the downloaded `flows.json` file.
11. Locate the `openweathermap` node. Paste the API key from step 7 into the API Key field in the node editor. Change other fields as desired.

### Dashboard
12. Copy the link from step 4, then add `ui` at the end (e.g. http://127.0.0.1:1880/ui).
13. Inject the `timestamp` node in the workspace to update the weather details to that of the current time.
    
    <img width="1920" height="827" alt="image" src="https://github.com/user-attachments/assets/5a27978a-35e9-4363-8bb4-df0fc386dbc3" />

15. (Optional) Modify the `timestamp` node to automate the injection at intervals.
    
    <img width="1920" height="827" alt="image" src="https://github.com/user-attachments/assets/56459616-c7ed-418a-af25-565192db61d4" />

## Resources

- References:
  - [Running on Windows: Node-RED](https://nodered.org/docs/getting-started/windows)
- Font: DotGothic16 [Google Fonts](https://fonts.google.com/specimen/DotGothic16/) [GitHub](https://github.com/fontworks-fonts/DotGothic16)
- Icons: https://openweathermap.org/weather-conditions

