![VSeeFace Minecraft](/vseeface-minecraft.gif)

# vseeface-minecraft
A Minecraft Avatar for VSeeFace. It uses my skin but I'll include hot to make your own.

## Using the Avatar
1. Download the [avatar](/Assets/Kirbycope.vrm)
1. Download [VSeeFace](https://www.vseeface.icu/#download) and unarchive.
1. In the VSeeFace folder, double-click on "VSeeFace.exe".
1. Select "Add Avatar" and select Kirbycope.vrm
1. Select "Start"

## How It was Made
- [Minecraft Vtuber Model! ✩ Tutorial](https://www.youtube.com/watch?v=kHda8H3eMcY) by Argama Witch
- I used [v0.58.0](https://github.com/vrm-c/UniVRM/releases/tag/v0.58.0) of UniVRM becuase it had documenation about [BlendedShapes](https://vrm.dev/en/univrm/export/univrm_export.html#v0-58) and that Argama was using VRM0 as well.
- [Minecraft Player Rig v2.0](https://vrcmods.com/item/5914) by aaronfranke

### How to Make it Your Own

#### Textures to Edit
Save your files to "/Assets/Kirbycope.Textures" for now. This will updated later when it's exported.
1. ["/Assets/Kirbycope.Textures/kirbycope.png"](/Assets/Kirbycope.Textures/kirbycope.png)
    - Remove the mouth as that'll be a seperate Unity layer (below)
1. ["/Assets/Kirbycope.Textures/Eye_Left_Closed.png"](/Assets/Kirbycope.Textures/Eye_Left_Closed.png)
1. ["/Assets/Kirbycope.Textures/Eye_Right_Closed.png"](/Assets/Kirbycope.Textures/Eye_Right_Closed.png)
1. ["/Assets/Kirbycope.Textures/mouth.png"](/Assets/Kirbycope.Textures/mouth.png)

#### Updating the Default Unity Model's Skin
[Unity](https://unity.com/) will be used to edit this `.vrm` model.
1. Open the project in Unity
    - This project uses "2021.3.19f1" as defined in ["/ProjectSettings/ProjectVersion.txt"](/ProjectSettings/ProjectVersion.txt)
1. In the Project view, selct "Assets" > "Kirbycope.Materials"
1. Select "UVmap2"
    - In the Inspector view, select the 🔘 between the texture preview and "Lit Color, Alpha", then select your texture
1. Repeat for "Eye_Left_Closed" and "Eye_Right_Closed"
1. The the Scene view, select the "Kirbycope" object
1. Select "VRM" > "UniVRM-0.58.0" > "Export Humanoid"
1. Enter a Name, Version, and Author
1. Select "Export"

#### Updating Your Model's Skin
Assuming you have completed the previous secion, "Updating the Default Unity Model's Skin".
1. Open the project in Unity
1. The the Scene view, select the "Kirbycope" object and delete it
    - Delete any remaing "Kirbycope" folders
1. Drag your `.vrm` file into the Assets View
1. Once imported, drag the Model into the scene
