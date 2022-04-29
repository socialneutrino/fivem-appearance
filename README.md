# sm-fivem-appearance

A modified version of brp version found here https://forum.cfx.re/t/brp-fivem-appearance/4170313 and ofcourse all credits go to https://forum.cfx.re/t/release-fivem-appearance/2438537

## Dependencies

- ESX 1.6
- zf Context Menu https://github.com/zf-development/zf_context
- NeroHiro’s Keyboard (Can be easily replaced) https://forum.cfx.re/t/release-standalone-nerohiro-s-keyboard-dynamic-nui-keyboard-input/2506326
- CD Draw text UI (Can be easily replaced) https://forum.cfx.re/t/free-release-draw-text-ui/1885313

## Conflicts

This rescorce is meant to replace these two so it cannot be used while these rescorces are running 
- esx_skin
- skinchanger

## Setup
- Run Outfits.sql
- Replace .css found in CD CSS with the one in cd_drawtextui\html\css
- Replace .css found in KEYBOARD CSS with the one found in nh-keyboard\ui

If you'r using esx_multicharacter or most rescorces using esx_skin or skinchanger this should work out of the box thansk to edits made by Linden however if it doeas not you can use the trigger below on the client side after the player loads in order to set their skin 

```cfg
ESX.TriggerServerCallback('fivem-appearance:getPlayerSkin', function(appearance)
    exports['fivem-appearance']:setPlayerAppearance(appearance)
end)
```

## Server Config

```cfg
ensure fivem-appearance
setr fivem-appearance:locale "en"
```

## Preview

![](https://i.imgur.com/w8IVP3I.png"")
![](https://i.imgur.com/aNkCAAQ.png"")
![](https://i.imgur.com/4rbAaY2.png"")

