---
layout: default
---

# Frequency asked questions

## My top is missing
KKBP applies the alphamask to the body by default. If your character is supposed to be a shirtless guy, you can open the Body Shader on the body material...

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq1.png)

and disable the "Built in transparency toggle" to show the top of the body

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq2.png)

If you're using multiple outfits, the alphamask may change based on the outfit. If you need to change the alphamask you can open up the Body textures node group on the body material...

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq3.png)

and change the alphamask to the body_AM_## file that corresponds to your outfit

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq4.png)

## My clothes are missing
During import, KKBP tries to automatically hide any extra clothes objects. Make sure the object wasn't accidentally hidden by checking the children of the Outfit object in the outliner

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq5.png)

## I'm getting fully white textures after importing my character
The import script failed somewhere. In Blender, click the Scripting tab on the top of the window. Any errors will appear at the bottom of the log. A successful import log will end in "KKBP import finished"

## I'm getting fully white textures, but only in certain places after importing my character
Some materials are supposed to have overlays, but KKBP cannot tell when that's supposed to happen, so it defaults to enabling overlays. Open the Shader of the clothes material that's showing up as white...

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq6.png)

Then try adjusting the sliders boxed below

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq7.png)

## My hair doesn't look right
Some hairs have "Maintex" textures, so KKBP will automatically make the Maintex active if it finds one. If that wasn't supposed to happen, open the Shader of the hair material...

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq8.png)

Then try adjusting the sliders boxed below

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq9.png)

## I got a "cf_pv_foot_L" / "cf_j_leg03_R" error during import
You accidentally chose the .pmx file inside of the "Outfit ##" folder instead of the .pmx file in the base export folder. Choose the correct .pmx file in the base export folder, or upgrade to KKBP 6.6+ (this version automagically makes sure you choose the right .pmx file).

## I upgraded to KKBP 6.6+ and still got a "cf_pv_foot_L" / "cf_j_leg03_R" error during import
Try importing again. It does that every once in a while.

## Blender crashed during import
Try importing again. It does that every once in a while.

## I don't know what versions of the programs or addons to use
KKBP has been updated many times to keep up with newer Blender versions, so the version of KKBP you need to use depends on what your Blender version is. [Check this table](https://github.com/FlailingFog/KK-Blender-Porter-Pack#required-software) for info on what versions to use.

## I'm using the right versions but it's still not working
Some heavily modded characters will not import correctly. Try exporting the default character that you get when you startup the character creator **with only the "Export Single Outfit" checkbox checked**, and [double check the table for choosing the right version](https://github.com/FlailingFog/KK-Blender-Porter-Pack#required-software). If that works, try adding back each piece of clothing / hair until the item that causes the issue is found. If that didn't work, [triple check you installed everything in the version table.](https://github.com/FlailingFog/KK-Blender-Porter-Pack#required-software)

![image](https://raw.githubusercontent.com/FlailingFog/flailingfog.github.io/master/assets/images/faq10.png)