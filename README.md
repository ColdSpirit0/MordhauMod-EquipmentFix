# Equipment Fix

Makes equipment from different mods compatible. Can be used as equipment loader.


## How to install
1. Create the directory `.../MORDHAUEditor/Mordhau/Mods/EquipmentFix`.
2. Move to the directory and open the command prompt.
3. Write `git clone https://github.com/ColdSpirit0/MordhauMod-EquipmentFix.git .`


## Config example

```ini
[/Script/Mordhau.MordhauGameSession]
Mods=3754454 ; https://mod.io/g/mordhau/m/equipment-fix

[/Script/Mordhau.MordhauGameMode]
SpawnServerActorsOnMapLoad=/EquipmentFix/EquipmentFixInit.EquipmentFixInit_C

[EquipmentLoader]
IsVerbose=False               ; Print debugging information about loaded equipment
StartDelay=0.5                ; Delay before loading equipment to game and starting to check for equipment changes
WatchDuration=20              ; How long to watch for equipment changes
RemoveVanillaItems=False      ; Remove vanilla items, useful for testing
LoadEquipment=/ModName/PathTo/BP_Weapon1.BP_Weapon1_C
LoadEquipment=/ModName/PathTo/BP_Weapon2.BP_Weapon2_C
```