## ABOUT

Just a **dhewm3** fork based on *Stradex*'s **unlockedFPS** patch (https://github.com/Stradex/dhewm3/tree/unlockedFPS) to bring the patched executables and libraries up-to-date with the mod's latest version.

To compile it yourself, follow the official **dhewm3** repo README instructions: https://github.com/dhewm/dhewm3/blob/master/README.md.

## INSTALLATION

These are the *recommended* steps to follow to install the patch, some of them are **[optional]**, but - for the best possible experience - I highly suggest you complete each and every single one of them:

1. Install Doom 3/RoE (I only tested Steam's version, but since it's based on dhewm3, physical should be fine as well)
2. **[optional]** Install D3EE (https://www.moddb.com/mods/doom-3-enhanced-edition)
3. Install dhewm3 **1.5.2** (https://dhewm3.org/) **in the main game's folder** (e.g.: "C:\Program Files (x86)\Steam\steamapps\common\Doom 3\\")
4. **[optional]** Install D3HDP (https://www.moddb.com/mods/d3hdp-doom-3-essential-hd-pack) - trust me.
5. Install **unlocked-fps-rw** (https://github.com/simonedibilio/dhewm3/releases) by replacing the executables and libraries in the main game's folder with the ones provided in the .zip file
6. Run the game once through the new dhewm3 executable
7. Once in the main menu, press **~** ; this will open the console and from here you want to type the command "**com_gameHz 120**" and press **ENTER** (I advise against setting anything higher than 120)
8. Exit the game
9. **[optional]** check out my suggested **CONFIGURATION** in the next paragraph and apply it to your autoexec.cfg file
10. Relaunch the game

## CONFIGURATION

After step 8 and before step 10 of the installation guide, you may want to apply the following settings to the **autoexec.cfg** file in your "..\Doom 3\base\" folder (if it's not there, just create it):

```
seta com_videoRam "4096" /* only if you have at least 8GB of VRAM, otherwise either 2048 (4GB+ of VRAM) or 1024 (2GB+ of VRAM)
seta r_swapInterval "0"  /* V-Sync bad, let's turn it off
seta r_fullscreen "1"    /* windowed should be fine, but fullscreen is better
seta com_preciseTic "0"
```

Everything else - including the resolution - should be settable in the game's "settings" menu.

## KNOWN ISSUES

- **Mods compatibility is broken**, only games playable are the two main ones, Doom 3 and Resurrection of Evil, for everything else (Classic Doom 3, The Lost Mission, etc.) you'll have to rely on "vanilla" dhewm3
- **Old save files are incompatible**
- There *may* be a problem with the patch that slows the game down to 24 FPS after playing the game for a while (1+ hours), which was present in Stradex's version; <ins>I haven't however encountered this issue on this port after playing for a couple of hours.</ins> If you **do** come across this issue though, all you have to is 1. save the game 2. restart it