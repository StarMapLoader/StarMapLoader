# Installing mods with StarMap

This page covers how to install mods that work with StarMap.

First make sure you installed StarMap via this guide: [StarMap installation guide](http://127.0.0.1:8000/KSAModding/getting-started/install-tools/#starmap-ksa-code-loader)

## How to install mods

1.  Download the mod's zip that contains the class library dll as well as any dependencies.
2.  Extract the zip folder so that the .dll file is inside a folder with the same nam as the .dll file.
    ```
        StarMap.ExampleMod
        └── StarMap.ExampleMod.dll
        └── ...
    ```
3. Put this folder inside of the game content files: `"KSAInstallLocation/Content/`, This folder should also contain the `Core` mod folder.
4. Lastly the mod needs to be added to the manifest.toml in the `"KSAInstallLocation"/Content/` folder, the id needs to match the name of the folder, the .dll file, the name variable inside mod.toml.
```
[[mods]]
id= "core"
enabled = true

[[mods]]
id = "[mod name]"
enabled = true
```
5. When now loading the game via `StarMap.exe` or `StarMapLoader.exe`, the mod should be loaded and run.
