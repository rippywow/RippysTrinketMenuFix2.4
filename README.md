# RippysTrinketMenuFix
Fix TrinketMenu having low render priority(Strata)

### Before

<img src="images/Rippys_TrinketMenu_Fix.png" width=300>

### After

<img src="images/Rippys_TrinketMenu_Fix1.png" width=300>

### Dependancies 

TrinketMenu

### How to install

Place Rippys_TrinketMenu_Fix into your addon folder.
Should work for all versions of wow where TrinketMenu also works.
Will not work without TrinketMenu installed as it uses it as a dependancy.
If you're using a different version of wow other than 2.4.3 and don't want it to say out of date/incompatible, open the .toc file and change `## Interface: 20400` (Representing patch 2.4) to whatever version of wow you're on
For example, `##Interface: 11200` would represent patch 1.12 (vanilla)
You can also edit core.lua if trinket menu is being hidden still from `SetFrameStrata("MEDIUM");` to `SetFrameStrata("HIGH");` giving it even higher priority. 

### Changelog

Literally just found out what TrinketMenu frames call themselves and slapped a `SetFrameStrata("MEDIUM");` onto them
babbys first addon btw
