# Clair-Obscur-Expedition-33-DOF-and-Fog-Fix-Windows-and-Linux
Fix for blurry DOF and fog in Clair Obscur: Expedition 33
1. Install the game

2. Run the game and set the settings however you like

3. Download Engine.ini from this repository

4. On Windows go into your ``C:\User\LOCAL\APPDATA\Sandfall\Saved\Config\Windows`` on Linux it will be ``/steamapps/compatdata/1903340/pfx/drive_c/users/steamuser/AppData/Local/Sandfall/Saved/Config/Windows``

5. Paste the Engine.ini file into the ``C:\User\LOCAL\APPDATA\Sandfall\Saved\Config\Windows`` on Linux into ``/steamapps/compatdata/1903340/pfx/drive_c/users/steamuser/AppData/Local/Sandfall/Saved/Config/Windows``

6. Check your GameUserSettings.ini file and Copy\Paste  everything into Engine.ini file after the lines below.

``[ScalabilityGroups]
sg.ResolutionQuality=100
sg.ViewDistanceQuality=3
sg.AntiAliasingQuality=3
sg.ShadowQuality=2
sg.GlobalIlluminationQuality=3
sg.ReflectionQuality=3
sg.PostProcessQuality=2
sg.TextureQuality=3
sg.EffectsQuality=3
sg.FoliageQuality=3
sg.ShadingQuality=3
sg.LandscapeQuality=0

[SystemSettings]
r.DepthOfFieldQuality=0
r.fog=0
r.VolumetricFog=0

[/script/engine.renderersettings]
r.ViewDistanceScale=5
r.SkeletalMeshLODBias=-2
r.StaticMeshLODDistanceScale=0.25``

7. Windows: save your Engine.ini file as read only on Windows.
8. Linux: type ``cd`` paste the path to your ``/steamapps/compatdata/1903340/pfx/drive_c/users/steamuser/AppData/Local/Sandfall/Saved/Config/Windows`` location
* ``sudo su``
* ``chattr +i Engine.ini``

Enjoy unblurred visuals on your OS of choice.

# silentgameplays


