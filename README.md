![VSeeFace Minecraft](/vseeface-minecraft.gif)

# vseeface-minecraft
A Minecraft Avatar for VSeeFace. It uses my skin but I'll include hot to make your own.

## Using the Avatar
1. Download the [avatar](https://github.com/kirbycope/vseeface-minecraft/raw/main/Kirbycope.vrm)
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
1. ["/Assets/Kirbycope.Textures/kirbycope.png"](/Assets/Kirbycope.Textures/kirbycope.png)
    - Replace with your avatar (sized 512x512)
    - Remove your avatar's mouth as that'll be a seperate Unity layer (below)
1. ["/Assets/Kirbycope.Textures/Eye_Left_Closed.png"](/Assets/Kirbycope.Textures/Eye_Left_Closed.png)
1. ["/Assets/Kirbycope.Textures/Eye_Right_Closed.png"](/Assets/Kirbycope.Textures/Eye_Right_Closed.png)
1. ["/Assets/Kirbycope.Textures/mouth.png"](/Assets/Kirbycope.Textures/mouth.png)

#### Exporting the VRM
[Unity](https://unity.com/) will be used to edit this `.vrm` model.
1. Open the project in Unity
    - This project uses "2021.3.19f1" as defined in ["/ProjectSettings/ProjectVersion.txt"](/ProjectSettings/ProjectVersion.txt)
1. In the Project view, select "Assets" > "Kirbycope.Materials"
1. The the Scene view, select the "Kirbycope" object
    - Double-check that the eyes and mouth line up with your model and adjust accordingly
1. Select "VRM" > "UniVRM-0.58.0" > "Export Humanoid"
1. Enter a Name, Version, and Author
1. Select "Export"
