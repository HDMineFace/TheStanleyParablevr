<div align="center">
  <p>
    <a align="center" href="https://store.steampowered.com/app/221910/The_Stanley_Parable/" target="_blank">
      <img width="auto" src="imgs/logo.png"></a>
  </p>
</div>

### All information is currently out of date and is the same as the original Portal2VR fork, this will eventually be updated.
# ![The Stanley Parable icon](imgs/icon.jpg "The Stanley Parable icon") The Stanley Parable VR
### ~~Use this mod at your own risk of getting VAC banned. Use the -insecure launch option to help protect yourself.~~
### The Stanley Parable doesn't have VAC, but just to be safe you should still run the game with the `insecure` flag.
This game contains flashing lights and fast motion sequences.

## Portal 2 VR Mod First 20 Minutes (Youtube Video)
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/nQZ601kEDFI/0.jpg)](https://www.youtube.com/watch?v=nQZ601kEDFI)

## Things that work
* Singleplayer
* 6DoF VR view
* Motion controls for portal gun and grabbable objects
* Workshop content

## Things that need fixing
* Use the game's own haptic feedback
* In-game UI and pause menu are broken
* 6DoF and Roomscale needs to be reimplemented
* CPU is underutilized

## How to use
1. Download [Portal2VR.zip](https://github.com/Gistix/portal2vr/releases) and extract the files to your Portal 2 directory (steamapps\common\Portal 2)
2. Connect your headset, then launch Portal 2 with these launch options:
   
   ``` -insecure -window -novid +mat_motion_blur_percent_of_screen_max 0 +mat_queue_mode 0 +mat_vsync 0 +mat_antialias 0 +mat_grain_scale_override 0 -width 1280 -height 720 ```

3. At the menu, feel free to change [these video settings](https://i.imgur.com/yYQMXs6.jpg).
4. Load into a chapter. 
5. To recenter the camera height, press down on the left stick. To see the HUD, aim the controller up or down.

## Troubleshooting
If you have no audio:
* Go to ```steamapps\common\Portal 2\portal2_dlc3``` and execute ```UpdateSoundCache.cmd```
  
If the game isn't loading in VR:
* Try opening SteamVR before the game
* Disable SteamVR theater in [Steam settings](https://external-preview.redd.it/1WdLExouo_YKhTGT6C5GGrOjeWO7qNdIdDRvIRBhw-0.png?auto=webp&s=0d4447a9d954e1ec15b2c010cf50eeabd51f4197)

If the game is stuttering, try: 
* Steam Settings -> Shader Pre-Caching -> Allow background processing of Vulkan shaders

If the game is crashing, try:
* Lowering video settings
* Disabling all add-ons then verifying integrity of game files
* Re-installing the game

## Build instructions
1. ``` git clone --recurse-submodules https://github.com/Gistix/portal2vr.git ```
2. Open l4d2vr.sln
3. Set to x86 Debug or Release
4. Build -> Build Solution

Note: After building, it will attempt to copy the new d3d9.dll to your Portal 2/bin directory.

## Based on
* [portal2vr](https://github.com/Gistix/portal2vr)
* [l4d2vr](https://github.com/sd805/l4d2vr)

  
## Utilizes code from
* [VirtualFortress2](https://github.com/PinkMilkProductions/VirtualFortress2)
* [gmcl_openvr](https://github.com/Planimeter/gmcl_openvr/)
* [dxvk](https://github.com/TheIronWolfModding/dxvk/tree/vr-dx9-rel)
* [source-sdk-2013](https://github.com/ValveSoftware/source-sdk-2013/)

