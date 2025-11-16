# Installing Tools

This page describes the basic tools you'll likely want when creating mods for KSA.

## Essentials

- A **text editor** (VS Code, Sublime Text, etc.) for editing config files and scripts.
- A **file archiver/browser** for inspecting game data if needed.
- The **KSA game** itself, installed in a location where you can access its files.

## StarMap (KSA Code Loader)

-   Download and unzip release from [Releases](https://github.com/StarMapLoader/StarMap/releases/latest).
-   Run StarMap.exe, this will fail and create a StarMapConfig.json.
-   Open StarMapConfig.json and set the location of your KSA installation.
    -   `GameLocation` should be set to the location where Kitten Space Agency was installed, pointing directly to that folder (e.g. `C:\\games\\Kitten Space Agency\\`)
    -   `RepositoryLocation` can be kept empty
-   Run StarMap.exe again, this should launch KSA and load your mods.

## Blender

1. Go to the [offical blender download website](https://www.blender.org/download/).
2. Download the installer for your OS (Windows, macOS, Linux)
3. Run the installer:
   - Windows: double-click .exe → follow prompts
   - macOS: drag Blender.app to Applications
   - Linux: extract tar.bz2 or use package manager
4. Open Blender

## KSA Mod Loader

1. Download and unzip KSA Mod Loader from [KSA Mod Loader](https://www.mediafire.com/file/kbh4jrd7iogk3mn/KSAModManager.zip/file)
2. Run the KSAModLoader.exe
3. Select "1" to enter in the paths to your Kitten Space Agency folders
    - `Manifest Path` should be set to your KSA folder that contains the manifest.toml (e.g. `C:\Users\    <username>\OneDrive\Documents\My Games\Kitten Space Agency`)
    - `Game Path` should be set to your actual Kitten Space Agency game files. (e.g. `C:\Program Files\Kitten Space Agency`)
    - NOTE: Do not put the file paths in quotes.
5. Paste the zip files for the mods you want to install into the ModSetup folder.
    - This can be done at any time to install new mods.
    - For the time being, copy and paste zipped mods into here, don't cut and paste, the Mod Manager deletes the zips to prevent accidental mod duplication after installation.
7. Go back to KSAModLoader.exe and select "2" to install mods.
8. To remove mods please select "3" and then the corrosponding number for the mod you want to remove.
