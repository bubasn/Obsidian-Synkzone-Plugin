Fully supports both linux and windows machines.

# Main Features:
* See sync status in the lower right corner when using obsidian
* Select target zone using a dropdown list
* Manually refresh sync check using a button on the left pane
* **For developers:** Toggle logging for in-depth troubleshooting in the obsidian console (CTRL + SHIFT + i)

## Before downloading:
1. Ensure you have the Synkzone desktop client downloaded on your computer.
2. Shutdown the Synkzone desktop client.
3. Open the file:
  **Windows:** C:\Users\<användarnamn>\AppData\Roaming\Synkzone Desktop\config.json
  **Linux:** Home/.config/Synkzone Desktop/config.json
4. Change "sz-backend-options": "" -> ```"sz-backend-options": "[\"-Dcom.synkzone.storage.data.displayTransferPanel=false\",\"-DmaxStorageSpace=3500000000\",\"-Dquarkus.http.cors=true\",\"-Dquarkus.http.cors.origins=*\",\"-Dquarkus.http.cors.access-control-allow-credentials=true\"]",``

## How to Download:
1. Go to releases and download the latest release.
2. Open Obsidian -> Settings -> Community plugins
3. Make sure restricted mode is off
4. Click on the folder to open the obsidian plugins folder. 
5. Move the Synkzone plugin folder into the obsidian plugin folder.
6. Unzip the file
7. Go back to obsidian and refresh the plugins + click enable on the plugin.

## How to Start:
1. After downloading, go to community plugins -> go to settings for the synkzone plugin. 
2. Configure the API port for your client and select which zone to target (Which zone obsidian uses)
