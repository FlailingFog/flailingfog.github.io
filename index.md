---
layout: default
---

## Usage Instructions for V7
1. Install the [HF Patch for Koikatsu](https://github.com/ManlyMarco/KK-HF_Patch), or the [HF Patch for Koikatsu Sunshine](https://github.com/ManlyMarco/KKS-HF_Patch). **Pre-modded repacks will not work** unless you update your plugins with KKManager or install the HF patch
1. Find your Koikatsu install directory and drag the KKBP exporter into the /bepinex/plugins/ folder
1. Start Koikatsu and open the Character Maker
1. You'll see this UI at the top now. If you are using KKS, you'll get the left panel. If you are using KK you'll get the right panel  
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/exportpanel.PNG)
1. Click the "Export Model for KKBP" button the top of the screen. This may take a few minutes depending on your computer hardware. A folder in your Koikatsu install directory will popup when the export is finished
1. Open Blender 4.2. **Other versions are not guaranteed to work**
1. Install [mmd_tools](https://extensions.blender.org/add-ons/mmd-tools/)
1. Install KKBP Importer 7.0.0
1. You'll see this UI in Blender now. Click on one of the buttons to allow KKBP to download an older version of blender  
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel1.PNG)
1. After it is done downloading, you can click the "Import model" button  
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel2.PNG)
1. Choose the .pmx file from the export folder 
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel3.PNG)
1. The blender console will appear and begin importing the model. This may take a few minutes depending on your computer hardware  
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel4.PNG)
1. Check there were no errors during import in the scripting tab. A successful import will end in "KKBP import finished in XX minutes"  
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel5.PNG)
1. You can start using the model as is, but it is recommended to finalize the materials first. If you use the model as is, it will take a long time to compile all the shaders. If you finalize the materials then the shaders will compile very quickly. It also makes the shaders compile quickly if you decide to reimport the same model.  
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel6.PNG)


The last known working configuration for **Koikatsu / Koikatsu Party** as of writing this text is HF Patch v3.28, Koikatsu 5.1, Blender 4.2.0, KKBP Importer 7.0.0, KKBP Exporter v4.30, mmd_tools 4.2.2  
The last known working configuration for **Koikatsu Sunshine** as of writing this text is HF Patch for KKS v1.17, Koikatsu Sunshine 5.1, Blender 4.2.0, KKBP Importer 7.0.0, KKBP Exporter v4.30, mmd_tools 4.2.2


#### Exporting from Blender to fbx:

1. Click the Finalize Materials button in the panel  
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel6.PNG)
1. This does three things
    * Bakes all of the materials to png files and saves them to the baked_files folder in your export folder
    * Creates an atlas file for your body / hair / clothes and saves them to the atlas_files folder in your export folder
    * Creates a new collection that uses the atlas
1. Hide the original collection in the outliner and show the new collection
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel7.PNG)
1. Click the "Prep for target application" button if you want to reduce the bone count or convert the model's armature for VRM / VRChat
1. Click the export button in the collection tab to export an fbx file to atlas_files in your export folder
![ ](https://github.com/FlailingFog/flailingfog.github.io/blob/master/assets/images/importpanel8.PNG)

## Wiki contents

### Frequently asked questions
* [My top is missing](faq#My-top-is-missing)
* [My clothes are missing](faq#My-clothes-are-missing)
* [I'm getting fully white textures after importing my character](faq#Im-getting-fully-white-textures-after-importing-my-character)
* [I'm getting fully white textures, but only in certain places after importing my character](faq#Im-getting-fully-white-textures-but-only-in-certain-places-after-importing-my-character)
* [My hair doesn't look right](faq#My-hair-doesnt-look-right)
* [I got a "cf_pv_foot_L" / "cf_j_leg03_R" error during import](faq#i-got-a-cf_pv_foot_l--cf_j_leg03_r-error-during-import)
* [I upgraded to KKBP 6.6+ and still got a "cf_pv_foot_L" / "cf_j_leg03_R" error during import](faq#i-upgraded-to-kkbp-66-and-still-got-a-cf_pv_foot_l--cf_j_leg03_r-error-during-import)
* [Blender crashed during import](faq#Blender-crashed-during-import)
* [I don't know what versions of the programs or addons to use](faq#I-dont-know-what-versions-of-the-programs-or-addons-to-use)
* [I'm using the right versions but it's still not working](faq#Im-using-the-right-versions-but-its-still-not-working)

### Panel options
* [Default panel settings](panel#Default-panel-settings)
* [Importing panel](panel#Importing-panel)
* [Exporting panel](panel#Exporting-panel)
* [Extras panel](panel#Extras-panel)

### Mesh features
* [Face shapekeys](mesh#Face-shapekeys)
* [Tear and gag eye shapekeys](mesh#Tear-and-gag-eye-shapekeys)
* [Body seams](mesh#Body-seams)
* [Object organization](mesh#Object-organization)

### Armature features
* [Armature layers](armature#Armature-layers)
* [Joint corrections](armature#Joint-corrections)
* [KKBP armature features](armature#kkbp-armature)
* [Rigify armature features](armature#rigify-armature)

### Material features
* [The KKBP material setup](material#The-KKBP-material-setup)
* [Plain Maintex vs Colored Maintex](material#Plain-Maintex-vs-Colored-Maintex)
* [Special materials (Outlines)](material#Special-materials-Outlines)
* [Special materials (Hair)](material#Special-materials-Hair)
* [Special materials (Eyes)](material#Special-materials-Eyes)
* [Special materials (Tears)](material#Special-materials-Tears)
* [Special materials (Gag eyes)](material#Special-materials-Gag-eyes)
* [Smoothing out the look of the face with Generated Face Normals (GFN)](material#Smoothing-out-the-look-of-the-face-with-Generated-Face-Normals-GFN)
* [Koikatsu color conversion](material#Koikatsu-color-conversion)
* [Koikatsu dark color conversion](material#Koikatsu-dark-color-conversion)
* [Cycles support](material#Cycles-support)
* [Lightning Boy Shader support](material#lightning-boy-shader-support)
* [Normal blending methods](material#Normal-blending-methods)
* [Normal quality settings](material#Normal-quality-settings)
* [Toon shading settings](material#Toon-shading-settings)
* [Permanent light / dark settings](material#permanent-light--dark-settings)
* [Per-character light linking settings](material#Per-character-light-linking-settings)
* [Light color influence](material#Light-color-influence)
* [Shader to RGB support](material#Shader-to-RGB-support)
* [Editing the KKBP shader](material#Editing-the-KKBP-shader)

### Misc
* [Getting info from the Koikatsu console](misc#Getting-info-from-the-Koikatsu-console)
* [Getting info from the Blender console](misc#Getting-info-from-the-Blender-console)
* [Baking materials](misc#Baking-materials)
* [Re-baking materials](misc#Re-baking-materials)
* [Working with Freestyle outlines](misc#Working-with-Freestyle-outlines)
* [Armatures in Unity](misc#Armatures-in-Unity)
* [Springbones in Unity](misc#Springbones-in-Unity)

### Manual test cases
[These test cases are the ones used to make sure the Blender addon works before a release is published.](standard_manual_test_cases)