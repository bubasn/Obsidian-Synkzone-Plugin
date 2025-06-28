# Synkzone Obsidian Plugin

A plugin that fully supports **Linux** and **Windows** for integrating Synkzone functionality directly into Obsidian.

## 🔧 Main Features

- ✅ Display sync status in the bottom-right corner of Obsidian  
- ✅ Select your target zone using a dropdown menu  
- ✅ Manually refresh sync status with a button in the left ribbon  
- ✅ **Developer Mode**: Enable detailed logging in the console (`Ctrl + Shift + I`)

---

## ⚠️ Prerequisites

Before installing the plugin, ensure the following:

1. You have the **Synkzone Desktop Client** installed.
2. You **shut down the Synkzone Desktop Client** before editing configuration files.
3. Locate and open your `config.json` file:
   ```text
   Windows: C:\Users\<your-username>\AppData\Roaming\Synkzone Desktop\config.json
   Linux:   ~/.config/Synkzone Desktop/config.json
4. Modify the `sz-backend-options` field as follows:

   ```json
   "sz-backend-options": [
     "-Dcom.synkzone.storage.data.displayTransferPanel=false",
     "-DmaxStorageSpace=3500000000",
     "-Dquarkus.http.cors=true",
     "-Dquarkus.http.cors.origins=*",
     "-Dquarkus.http.cors.access-control-allow-credentials=true"
   ]

## ⬇️ Installation

1. Go to the [Releases](https://github.com/bubasn/Obsidian-Synkzone-Plugin/releases/tag/V1.0.0) section and download the latest `.zip` release.
2. In Obsidian:
   - Open `Settings → Community plugins`
   - Turn off **Restricted mode**
3. Click **"Open plugins folder"**.
4. Move the **unzipped Synkzone plugin folder** into the opened folder.
5. Return to Obsidian:
   - Click **"Reload plugins"**
   - Enable the **Synkzone** plugin

## 🚀 Getting Started

1. In Obsidian, go to:  
   `Settings → Community plugins → Synkzone Plugin`
2. Configure the plugin:
   - **API Port** for your Synkzone client
   - **Target Zone** that Obsidian should sync with

## 🛠 Developer Options

- Toggle **Developer Logging** in the plugin settings.
- When enabled, internal logs will appear in the **Developer Console**.
- Open the console with: `Ctrl + Shift + I`.

## ✅ Compatibility

- **Operating Systems:**
  - Windows
  - Linux

## 🙋 Support

Have questions or issues? Please [open an issue](../../issues) in this repository.

