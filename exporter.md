---
layout: default
---

# Exporter Panel settings
Each setting in the exporter panel will be briefly detailed on this page.  
If you are using KKS, you'll get the left panel. If you are using KK you'll get the right panel  
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/exportpanel.png)


### Export variations

This will export any available clothing variations. Not all clothes have variations.  
When imported, the variations will be hidden in the outliner by default.

![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/exporter1.png)

### Export hit meshes

This will export the hit mesh. An example of the hit mesh is shown below.

![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/exporter2.png)

### Export single outfit

This will make the exporter only export a single outfit, so if you only want one outfit this will dramatically increase your koikatsu export times and blender import times.

### Export without physics

Some outfits rely on in-game physics to look correct. Enable this option to disable the in-game physics during export. This may make certain outfits look weird because of the lack of physics, but it is useful if you want to apply your own physics to the model in blender.

### Enable pushups (KK only)

Pushups are disabled during export. Enable this option to re-enable pushups.

### Enable shapekeys (KK only)

Shapekeys are reverted to their default values during export. Enable this option to apply any shapekeys you have enabled in the character maker to the base mesh. Because the mesh is pre-deformed, other shapekeys will not work correctly in blender. Tear and gag eye shapekeys will also not work in blender. See the picture below for an example of some shapekeys being pre-applied to the base mesh. 

![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/exporter3.png)

### Keep current pose (KK only)

The pose is reset to a T pose during export. Enable this option to keep the pose you have selected in the character maker to the base mesh. Because a pose is already applied to the armature, the armature will not work correctly in blender. This setting may be useful for 3D prints of koikatsu models. This setting will force the Koikatsu armature in blender. See the picture below for an example of a pose being applied to the model. 

![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/exporter4.png)
