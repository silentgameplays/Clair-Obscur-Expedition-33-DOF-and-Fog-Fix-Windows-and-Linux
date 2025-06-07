# Fix for blurry DOF and fog in Clair Obscur: Expedition 33

1. Install the game

2. Run the game and set the settings however you like

3. Disable the blurry stuff like:

# Lens Flare

# Chromatic Aberration

# Film Grain

# Motion Blur

#NB! For a clear picture before applying this fix and use TSR at 100% or 75%, it will still lag heavily in one area called Yellow Harvest, everywhere else should be fine with 100/75 % TSR

4. On Windows go into your
``C:\User\LOCAL\APPDATA\Sandfall\Saved\Config\Windows``


5. On Linux it will be
`` /steamapps/compatdata/1903340/pfx/drive_c/users/steamuser/AppData/Local/Sandfall/Saved/Config/Windows ``

6. Open your GameUserSettings.ini file and copy\paste the code below into GameUserSettings.ini file after the ``[ScalabilityGroups]`` section and before your settings:

``[SystemSettings]
r.DepthOfFieldQuality=0
r.fog=0
r.VolumetricFog=0

[/script/engine.renderersettings]
r.ViewDistanceScale=5
r.SkeletalMeshLODBias=-2
r.StaticMeshLODDistanceScale=0.25``


7. On Windows: save your modified GameUserSettings.ini as Engine.ini file and make it as Read Only by right clicking on Properties.

8. Linux: save your modified GameUserSettings.ini as Engine.ini file. To make it read-only type
* ``cd`` 
# paste the path to your
``/steamapps/compatdata/1903340/pfx/drive_c/users/steamuser/AppData/Local/Sandfall/Saved/Config/Windows``
location

* ``sudo su ``

* ``chattr +i Engine.ini``


# Example of what your newly created Engine.ini should look like on top:

