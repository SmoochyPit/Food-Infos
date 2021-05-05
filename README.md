# Food Infos

Food Infos is a data pack for Minecraft: Java Edition which displays information about the food item currently being held. It is designed to work alongside [Item Infos](https://github.com/SmoochyPit/Item-Infos) or as a standalone data pack.

![Certified Compatibility + Stamp of Quality](https://i.imgur.com/ltLPoQp.png)
([Datapack Conventions?](https://mc-datapacks.github.io/en/))

## About 

### Features

* Food display with symbols for how many hunger bars the item replaces
    * Detailed food display with hunger and saturation as numbers
* Custom color configuration
* Custom symbol configuration
* Custom food item configuration
* Support for off-hand

### Other

**Potential Lag Notice**: When a player is holding a food item, the data pack must check to see if the player is holding each of the included food items. This is the equivalent of a massive chain of "if" statements. If you are running a server with a consistently large amount of players, many complex data packs or many food items (which you have included in the config file), please consider using a mod or plug-in.

I know the name is grammatically incorrect. It's just the style I chose :grin:

## Usage

Information is displayed based on what item you are holding and whether you are sneaking.

Holding a piece of food while not sneaking:
![Steak hunger display](https://i.imgur.com/QATGNEN.png)
![Bread hunger display](https://i.imgur.com/lSjG7sG.png)

Holding a piece of food while sneaking:
![Steak detailed hunger display](https://i.imgur.com/w7TBIm8.png)
![Bread detailed hunger display](https://i.imgur.com/cndqvTS.png)

## Installation
### Step 1 - Download

(If you are on a Unix-based operating system, run `wget $(curl -s https://api.github.com/repos/SmoochyPit/Food-Infos/releases/latest | grep 'browser_' | cut -d\" -f4)` in the datapacks folder of your world)

1. Click [releases](https://github.com/SmoochyPit/Food-Infos/releases)
2. Find the latest release
3. Under assets, click "food-infos-vX.X.zip" to download the data pack. *This file **should not** be unzipped before installation*
4. Select one of the following methods for installing the data pack:

### Step 2 - Data pack menu (New singleplayer worlds) (Very Easy)

1. In the Singleplayer menu, click "Create New World"
2. Click "Data Packs"
3. Drag the downloaded file onto your Minecraft window (toggle fullscreen with F11)
4. Click "Yes"
5. Hover over Food Infos in the menu and click the right arrow to add it to the list of selected data packs
6. Click "Done" and change any other world options you want
7. Click "Create New World"

### Step 2 - Manual installation (Existing singleplayer or multiplayer worlds) (Easy)

1. Place the downloaded file into the `[worldname]\datapacks` folder on your server or singleplayer world (located at `C:\Users\[user]\AppData\Roaming\.minecraft\saves\[worldname]\datapacks` by default in Windows)
2. Either restart the world or server, or run the `/reload` command.

At this point, Food Infos will now be installed in your Minecraft world.

### Support

Supports Minecraft: Java Edition 1.16-1.16.5. I plan to maintain this data pack for the 1.17 snapshots.

### Uninstalling

To uninstall, run `/function smoochypit:foodinfos/uninstall`. This will remove all objectives created by the data pack.

### Configuration

Configuration is handled by Trident during compilation. To compile the modified version of the data pack, you will need either [Trident UI](https://github.com/Energyxxer/Trident-UI) or [Trident Language](https://github.com/Energyxxer/Trident-Language).

1. Download and extract the source code
    * If using Trident UI, place this folder in your workspace folder
2. Change the output location in the file `.tdnproj`
    * If using Trident UI, this option is found under `File > Project Properties > Output > Data Pack Output` (Make sure to select the project in the explorer panel)
3. Config is located at `datapack\data\smoochypit\functions\foodinfos\config.tdn`
4. Compile the project (Alt-Shift-X in Trident UI)

## Credits

This data pack was inspired by https://github.com/squeek502/AppleSkin.

Created with http://energyxxer.com/trident/. (https://github.com/Energyxxer/Trident-UI)

Made with love by @SmoochyPit
