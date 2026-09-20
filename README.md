# 🛠️ FiveM Enhanced: Addon Vehicles & Custom Maps Fix

> A quick workaround for server owners and developers experiencing loading failures or console errors when streaming custom maps and addon vehicles in **FiveM Enhanced**.

## ⚠️ The Problem
When adding custom content (vehicles, maps) using the modern `cerulean` manifest version, the server may fail to load the resources properly or throw metadata errors in the console.

## ✅ The Solution
Changing the resource manifest version to `bodacious` resolves the loading errors for these assets. 

### Update your `fxmanifest.lua`
Replace your current manifest header with the following configuration:

```lua 
fx_version 'bodacious'
game 'gta5'

files {
    'vehicles.meta',
    'carvariations.meta',
    'handling.meta'
}

data_file 'VEHICLE_METADATA_FILE' 'vehicles.meta'
data_file 'VEHICLE_VARIATION_FILE' 'carvariations.meta'
data_file 'HANDLING_FILE' 'handling.meta'
```
[![Support me on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/zapproject)[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zapprojectrp)
