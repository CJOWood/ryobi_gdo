## Ryobi Garage Door Opener - HA Custom Component

This integration will request all of the Garage Door devices linked to your Ryobi account and automatically add them into Home Assistant, through a standard config flow.

The Garage Door must first be setup and added through Ryobi's app. Once you've created an account and can successfully control the garage door from the app, you can use your login details with this integration.

## Installation.

### Install from HACS (recommended)

1. Have [HACS][hacs] installed, this will allow you to easily manage and track updates.
2. Search in HACS for "Ryobi (When its added)" integration.
3. Add [https://github.com/catduckgnaf/ryobi_gdo](https://github.com/catduckgnaf/ryobi_gdo) as custom respository.
4. Click Install below the found integration.

# Issues

Please open an Issue and paste DEBUG logs or I can't help as easily. PLEASE remove all personal login details, including your username, password, device IDs, and API Keys!!



### Functionality / To-Do 
 - [x] HTTP: Login to check details and get API Key.
 - [x] HTTP: Get devices list to check for more than 1 GDO.
 - [x] HTTP: Get device state for each device.
 - [x] WS: Authenticate using API Key.
 - [x] WS: Subscribe to device notifications using device ID.  
 - [x] WS: Listen for device updates and update internal state.
 - [x] Implement RyobiGarage CoverEntity in HA.
 - [x] Set the unique_id properly using device_id, mac, serial and name.
 - [x] WS: Send open/close command to sever
 - [ ] Support Vacation mode toggle
 - [ ] WS: Check for and implement set_position command (look into app's "preset" functionality).
 - [ ] WS: Check for and implement stop command.
 - [x] Implement RyobiGarage LightEntity in HA.
 - [x] Implement Motion Sensor in HA.
 - [x] Fully Support G125
 - [-] Get identities for all modules. (currently a work in progress.).
### 'Thank You's
 - [Madj42](https://github.com/Madj42) and his [ryobi_gdo3](https://github.com/Madj42/ryobi_gdo3) integratio.
 - [**Jezza34000**](https://github.com//CJOWood/) and his [**Ryobi Garage**](https://github.com/CJOWood/ryobi_garage/) for initial websocket work.
 - [**firstof9**](https://github.com//firstof9/) and his enthusium for helping with this project.
