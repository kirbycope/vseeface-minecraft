## VRM
1. Download [VseeFace](https://www.vseeface.icu/)

### VRoid Studio
1. Install [VRoid Studio](https://vroid.com/en/studio)
1. Open VRoid Studio
1. Under Sample Models, select "AvatarSample_C"
1. Select 📤(Export) > "Export as VRM"
1. Select "Export"
1. Give the avatar a Title and name its Creator
1. Scroll down and select "Export"
1. Select your file save location and then select "Save"
1. Close VRoid Studio

### Unity
1. Install [Unity](https://unity.com/download)
	- Check that you are using a [recommended version](https://github.com/vrm-c/UniVRM#supported-environments)
1. Select "New project"
1. Select "3D (Core)"
1. Select "Create project"
1. After the project loads, select "Edit" > "Project Settings..."
1. In the left-nav, select "Player"
1. Expand "Other Settings" section
1. Under "Rendering" > "Color Space", select "Linear"
1. Close the settings window
1. Download [UniVRM](https://github.com/vrm-c/UniVRM/releases)
1. Select "Assets" > "Import Package" > "Custom Package"
1. Select the downloaded unity package and then select "Import" in the pop-up
1. Download [Minecraft Player Rig v2.0](https://vrcmods.com/item/5914)
1. Select "Assets" > "Import Package" > "Custom Package"
1. Select the downloaded unity package and then select "Import" in the pop-up
1. Drag and drop "Assets/Minecraft/MinecraftSteve" into the scence
1. Drag and drop "Assets/Minecraft/Materials/UVmap2" onto the model
1. In the properties change the "Shader" to "VRM" > "MTOON"
1. Save your skin to "Assets/Minecraft/Skins"
	- Your skin should be resized to 512x512
	- Create 24x24 eye textures; Eye_Right_Closed and Eye_Left_Closed
	- Create 16x8 mouth texture
1. Select the material map again
1. Click the small circle between the layer preview and the layer name
1. Select your player skin
1. Expand the MinecraftSteve model in the scence pane
	- "MinecraftSteve" > "Armature" > "Hips" > "Spine" > "Chest" > "Neck" > "Head"
1. Right-click "Head" and select "3D Object" > "Plane"
1. Rotate the plane by `90` on the x-axis
1. Scale the plane down to `0.00045` `0.000225` `0.000225`
1. Use the move tool to move the plan over the avatar's mouth
1. Rename the plane to `EI`
	- It will serve as the mouth shape for the sounds "E" and "I"
1. Copy that plane, make a mouth shape for `A`
1. Copy that plane, make a mouth shape for `U`
1. Copy that plane, make an eye shape for `Eye_Right` (your left)
1. Copy that plane, make an eye shape for `Eye_Left` (your right)
1. Copy the eye closed textures to the Minecraft folder
1. Select the Eye_Right from the stage pane
1. Change the texture and shader
	- Texture: Eye_Right_Closed
	- Shader: VRM/MTOON
	- Rendering Type: Cutout/Back
1. Repeat for the left eye
1. Copy the mouth texture to the Minecraft folder
1. Select "EI" from the stage pane
1. Change the texture and shader
	- Texture: mouth
	- Shader: VRM/MTOON
	- Rendering Type: Cutout/Back
1. Change each other letter by dragging the mouth material to the shape in the stage pane
1. Select each of the new Materials and move the Alpha slider to 1
1. Select "Export"
	- C:\Users\kirby\My project\Kirbycope.vrm
1. Select the MincraftSteve model in the scence pane
1. Select "VRM1" > "Export VRM-1.0"
	- Enter your avatar's name under "Name"
	- Enter your name under "Element 0"


1. Download https://github.com/vrm-c/UniVRM/releases/tag/v0.58.0
	- Referenced here, https://vrm.dev/en/univrm/export/univrm_export.html
1. Remove all VRM and Shader folders
1. Install 0.58.0
1. Export Humanoid
1. Go to BlendShapes in "Assets/Kirbycope"
1. Select "A"
1. Select "Material List"
1. Click "+"
1. In the first drop-down, select "A"
1. In the second drop-down, selct "_Color"

THE PROBELM SEEMS TO BE I MISWSED THE EXPORT AND REIMPOT of the VRM. @6:09 https://www.youtube.com/watch?v=kHda8H3eMcY ??







https://vrm.dev/en/univrm/import/univrm_import.html

https://www.youtube.com/watch?v=kHda8H3eMcY
	https://vrcmods.com/item/5914
		## Description
		Supports the latest skin format in 1.14 including jacket/etc all over the body.
		Sketchfab link: https://sketchfab.com/3d-models/minecraft-player-rig-v20-93fdf912488e48bbb428a5623664ae77
			- Based on https://vrcmods.com/item/3291
				- Which is based on https://www.youtube.com/watch?v=fFiCdLPnTjI
		## HOW TO USE
		1. Add your Minecraft skin in the "Skins" folder.
		2. Change import settings for your skin. You want to set it up just like the other skins: Enable "Alpha Is Transparency", disable "Generate Mip Maps", set "Wrap Mode" to "Clamp", set "Filter Mode" to "Point (no filter)", and set "Compression" to "None".
		3. If you want your avatar to have emission or specular textures, do the same as above, but disable "Alpha Is Transparency".
		4. Create a new material for your skin. You want to set it up just like the other skins: Set "Shader" to "Standard (Specular setup)", set "Rendering Mode" to "Cutout", and assign textures as needed.
		5. Create a new scene. Copy the contents of another scene to get started. Rename the object names and background text, and set the material in the character's "Body" -> "Skinned Mesh Renderer" -> "Materials" -> "Element 0".
		6. Upload the avatar and enjoy!
		Please do not use my "aaronfranke" skin, it is just there to be an example of how the rig works.
