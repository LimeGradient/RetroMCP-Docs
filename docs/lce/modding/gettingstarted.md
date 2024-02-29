# Getting Started

Modding Minecraft Legacy Console Edition is a fairly complicated task. We will be using a library called CodeLib written by David-xF and PhoenixARC to mod our game. These mods are called Graphic Packs on Cemu but for simplicity we will be calling them mods.  
WARNING: These mods will only work on the Cemu emulator.  

## Setting up the Workspace
What you will need:  
    - [CodeLib](https://github.com/David-xF/CodeLib)   
    - [devkitPro](https://devkitpro.org/wiki/Getting_Started)  
    - [Python](https://www.python.org/)  

1. Install devkitPro and Python using the links above.
2. Get CodeLib from the link above and extract it into your working directory
3. Go into the directory with CodeLib and run `make all`

After building, your mod will be found in `./GraphicPack`. You can put this in your `Cemu/graphicPacks` folder and it will be recognized by Cemu.