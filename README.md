# Equipment Fix

Makes equipment from different mods compatible. Can be used as equipment loader.


## How to install
1. Create the directory `.../MORDHAUEditor/Mordhau/Mods/EquipmentFix`.
2. Move to the directory and open the command prompt.
3. Write `git clone <url> .`


## Config example

```ini
; [/Script/Mordhau.MordhauGameSession]
; Mods= ; url

[/Script/Mordhau.MordhauGameMode]
SpawnServerActorsOnMapLoad=/EquipmentFix/EquipmentFixInit.EquipmentFixInit_C

[EquipmentLoader]
IsVerbose=False               ; Print debugging information about loaded equipment
StartDelay=0.5                ; Delay before loading equipment to game and starting to check for equipment changes
WatchDuration=20              ; How long to watch for equipment changes
RemoveVanillaItems=False      ; Remove vanilla items, useful for testing
```