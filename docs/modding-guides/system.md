# System
## Making a System File
A system file is a file that contains all the data of your system. The naming conventions for these files is that they are the name of the system you are making. An example of a system file is shown below. The file should be in .xml suffix.
```xml
<System Id="KerbolOnly">
<DisplayName Value="KSP System - Kerbin+Mun+Minmus Only"/>

<VesselTextures Size="184 MB">
<Texture Width="4096" Height="4096" Count="12" Size="181 MB"/>
<Texture Width="512" Height="512" Count="3" Size="3 MB"/>
</VesselTextures>
<TerrainTextures Size="2 GB">
<Texture Width="16384" Height="8192" Count="4" Size="0.8 GB"/>
<Texture Width="10800" Height="5400" Count="1" Size="37 MB"/>
<Texture Width="8192" Height="4096" Count="3" Size="277 MB"/>
<Texture Width="4096" Height="4096" Count="18" Size="1 GB"/>
<Texture Width="4096" Height="2048" Count="2" Size="64 MB"/>
<Texture Width="2048" Height="2048" Count="1" Size="16 MB"/>
<Texture Width="2048" Height="1024" Count="1" Size="8 MB"/>
<Texture Width="8" Height="8" Count="2" Size="512 B"/>
</TerrainTextures>
<UnscaledTextures Size="8 MB">
<Texture Width="128" Height="8192" Count="1" Size="4 MB"/>
<Texture Width="1024" Height="1024" Count="1" Size="4 MB"/>
<Texture Width="64" Height="64" Count="1" Size="16 KB"/>
<Texture Width="8" Height="8" Count="3" Size="768 B"/>
<Texture Width="1" Height="1" Count="2" Size="8 B"/>
</UnscaledTextures>
<LoadFromLibrary Id="Kerbol"/>
<LoadFromLibrary Id="Kerbin" Parent="Kerbol"/>
<LoadFromLibrary Id="Mun" Parent="Kerbin"/>
<LoadFromLibrary Id="Minmus" Parent="Kerbin"/>
<LoadFromLibrary Id="Rocket" Parent="Kerbin"/>
<LoadFromLibrary Id="Jeb" Parent="Kerbin"/>
</System>
```
## System ID and Display Name
A system ID is what the game will read your system as when loading the game. If two systems have the same ID, the game will load the one who's file name (not display or ID) no matter which system is selected.

A display name, however, does not matter, and can be anything. You're display name can contain any character you want and can be the exact same as another system file, the game will not care.
## Loading Planets
To load an Astronical file, the first object loaded should be your origin object (usually the Sun). Everything after that must have its parent assigned to it. Bodies who have planets assigned to them in this file will always orbit the body assigned in this file, even if it is different in  your Astronomicals file. 

If you want two different bodies to have the same name, it is recommended to add a space to the end of one of their names. It is possible to make custom fonts for special characters (allowing you to make an invisible letter or a letter that looks exactly like another), however it is not currently known how.
## Making Sure Your Systems Work
It is very common for your system to not appear when you start the game, even if your mod is enabled. This is usually because you forgot to define it in your mod.toml file. An example of multiple systems being defined in one mod is listed below.
```xml
systems = ["Kerbol.xml", "StockSystem.xml", "OPM.xml" ]
```