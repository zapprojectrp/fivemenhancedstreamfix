### For Owners/Devs whose servers fail to load or throw errors when adding custom maps or addon/custom vehicles to **FiveM Enhanced**, I’ve found a way to get them working.

In the **fxmanifest.lua**:

```
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

Use the [bodacious (2020-02)](https://docs.fivem.net/docs/scripting-reference/resource-manifest/#fx-version-cerulean-2020-05) version instead of the [cerulean  (2020-05)](https://docs.fivem.net/docs/scripting-reference/resource-manifest/#fx-version-cerulean-2020-05) one.


I don't know why, but this works on my server.
If anyone knows of any other solution, please share it. 
I hope this helps you!!
