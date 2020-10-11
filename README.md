# Windows-10-post-installation-cheatsheet
* enable HPET in UEFI/BIOS
```
useplatformclock        NO 
useplatformtick         Yes
disabledynamictick      Yes
```
```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Microsoft\GameBar] 
"ShowStartupPanel"=dword:00000000 
"GamePanelStartupTipIndex"=dword:00000003 
"AllowAutoGameMode"=dword:00000000 
"AutoGameModeEnabled"=dword:00000000 
"UseNexusForGameBarEnabled"=dword:00000000

[HKEY_CURRENT_USER\System\GameConfigStore] 
"GameDVR_Enabled"=dword:00000000 
"GameDVR_FSEBehaviorMode"=dword:00000002 
"GameDVR_FSEBehavior"=dword:00000002 
"GameDVR_HonorUserFSEBehaviorMode"=dword:00000001 
"GameDVR_DXGIHonorFSEWindowsCompatible"=dword:00000001 
"GameDVR_EFSEFeatureFlags"=dword:00000000 
"GameDVR_DSEBehavior"=dword:00000002

[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\GameDVR] 
"AllowGameDVR"=dword:00000000

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\GameDVR] 
"AppCaptureEnabled"=dword:00000000
```
