# Get Heroes of the Storm models & animation for Irrlicht

## Prerequisite

### Get SFM models
Download the model-pack from [SFMlabs](https://sfmlab.com/item/503/), thanks to Yaron for his work.

### Get Blender
Install Blender from [Blender-Download](https://www.blender.org/download/).

### Get Blender Source Tools
Install it from [Blender Source Tools website](http://steamreview.org/BlenderSourceTools/).

### Get B3D script
1. get B3D export script from [here](http://www.rtsoft.com/forums/showthread.php?7509-Blender-B3D-2-6x-Export-script).
2. Same install as Blender Source Tools.

### Get WinRAR
Get WinRAR form [WinRAR](https://shop.win-rar.com/16/purl-shop-1984-1-n?x-source=31-buybutton-startpage).

### Get Crowbar
Get Crowbar from [Crowbar - Source Engine Modding Tool](http://steamcommunity.com/groups/CrowbarTool), thanks to the members of the group for their work.

### Get .NET Framework Version 1.1
Get .NET Framework 1.1 from [Microsoft](https://www.microsoft.com/fr-fr/download/details.aspx?id=26).

### Get VTFEdit
Get VTFEdit from [Nem's Tools website][http://nemesis.thewavelength.net/index.php?p=41], thanks to [Nem](http://nemesis.thewavelength.net/index.php?a=1).

## Get 3D Model with Animation and Texture

### Unzip
Unzip Models and Materials you need.
There is a lot of ressources, the whole pack have a size of 8.1Go.
- Effects
- Heroes
- Mercs
- Minions
- Mounts
- Pets
- Props
- UI

### Convert Textures and Map
1. Run VTFEdit.
2. Tools>Convert Folder.
3. Select the Materials forlder you want to convert (for exemple : materials>models/HotS/Heroes).
4. Select the destination folder of converted files.
5. Select `to jpg` option, keep the `*vtf` box.
6. Set `Recursive` true.

### Convert .mdl to .qc and .smd
1. Run Crowbar.
2. Go to Decompile tab.
3. Select the `.mdl` of the model you want.
4. Select the `Full Path` of the destination folder.
5. Keep default setting, and Decompile.

## Convert .mdl to .b3d

### First Step
1. Run Blender.
2. Cancel the popup.
3. Hover the 3D view with mouse then delete the cube mesh with x>enter.
4. File>Import>Sources Engine.
5. Select the .qc in the decompiled folder of 3d models you get with Crowbar.

### Second Step
1. Set the `Editor Type` to `Dope Sheet`.
![dope sheet editor](https://cloud.githubusercontent.com/assets/9381120/26372608/cf668cc0-3ffe-11e7-8b4f-7d09deeb0139.PNG)
2. Set the Editor `Mode` to `Action Editor`.
![editor mode](https://cloud.githubusercontent.com/assets/9381120/26372674/f911a4b0-3ffe-11e7-9578-4b7b74e81d8c.PNG)
3. Prepare a spreadsheet to save lenght of all animation.
![animation timer](https://cloud.githubusercontent.com/assets/9381120/26372676/f9136156-3ffe-11e7-9ecc-026369645884.PNG)

### Third Step
1. Select all bones (shortcut `a` when hover bones with mouse).
![bone selection](https://cloud.githubusercontent.com/assets/9381120/26372675/f9135c38-3ffe-11e7-8b5e-1d61f00792a7.PNG)
2. Add in the linked animation all animation you want, in the correct order (select all keyframe with shortcut `a` when mouse hover the Action Editor).
3. Export the model in `.b3d` (Files>Export>B3D).

# You Win !
![victory](https://cloud.githubusercontent.com/assets/9381120/26372677/f9139b8a-3ffe-11e7-8c9d-3fe81162a6f2.PNG)
