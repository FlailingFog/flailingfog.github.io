---
layout: default
---

## Usage Instructions for V7
*The last known working configuration for **Koikatsu / Koikatsu Party** as of writing this text is HF Patch v3.28, Koikatsu 5.1, Blender 4.2.0, KKBP Importer 7.0.0, KKBP Exporter v4.30, mmd_tools 4.2.2  
The last known working configuration for **Koikatsu Sunshine** as of writing this text is HF Patch for KKS v1.17, Koikatsu Sunshine 1.1.4, Blender 4.2.0, KKBP Importer 7.0.0, KKBP Exporter v4.21, mmd_tools 4.2.2*  

1. Install the **[HF Patch for Koikatsu](https://github.com/ManlyMarco/KK-HF_Patch)**, or the **[HF Patch for Koikatsu Sunshine](https://github.com/ManlyMarco/KKS-HF_Patch)**.  
**Pre-modded repacks will not work** unless you update your plugins with KKManager or install the HF patch
1. Find your Koikatsu install directory and drag the KKBP exporter into the /bepinex/plugins/ folder
1. Start Koikatsu and open the Character Maker
1. You'll see this UI at the top now. If you are using KKS, you'll get the left panel. If you are using KK you'll get the right panel  
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/exportpanel.png)
1. Click the "Export Model for KKBP" button the top of the screen. This may take a few minutes depending on your computer hardware. A folder in your Koikatsu install directory will popup when the export is finished
1. Open Blender 4.2. **Other versions are not guaranteed to work**
1. Install **[mmd_tools](https://extensions.blender.org/add-ons/mmd-tools/)** in Blender
1. Install KKBP Importer 7.0.0 in Blender
1. You'll see this UI in Blender now. Click on one of the buttons to allow KKBP to download an older version of blender  
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/importpanel1.png)
1. After it is done downloading, you can click the "Import model" button  
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/importpanel2.png)
1. Choose the .pmx file from the export folder 
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/importpanel3.png)
1. The blender console will appear and begin importing the model. This may take a few minutes depending on your computer hardware  
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/importpanel4.png)
1. Check there were no errors during import in the scripting tab. A successful import will end in "KKBP import finished in XX minutes"  
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/importpanel5.png)
1. If there were no errors, you can start using the model as is, but it is recommended to finalize the materials first. If you use the model as is, it will take a long time to compile all the shaders. If you finalize the materials then the shaders will compile very quickly. It also makes the shaders compile quickly if you decide to reimport the same model. Finalizing the materials can take a few minutes depending on your hardware  
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/importpanel6.png)
1. If something doesn't look right and you don't see any errors in the log, check the [Wiki Home on the sidebar](wiki).

#### Exporting from Blender to fbx:

1. Click the Finalize Materials button in the KKBP panel  
1. This does three things
    * Finalizes all of the materials to png files and saves them to the baked_files folder in your export folder
    * Creates an atlas file for your body / hair / clothes and saves them to the atlas_files folder in your export folder
    * Creates a new collection that uses the atlas
1. Hide the original collection in the outliner and show the new collection
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/importpanel7.png)
1. Click the "Prep for target application" button if you want to reduce the bone count or convert the model's armature for VRM / VRChat
1. Click the export button in the collection tab to export an fbx file to atlas_files in your export folder
![ ](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/importpanel8.png)
