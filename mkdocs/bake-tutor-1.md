# Quick Guide How to Bake Normal Map

## Prepare UVs

First, make sure that you have UVs good for baking normal maps. This tutor is not about making UVs (it would require a separate book), so we assume that the reader is already familiar with this theme. In short:<br />
UV shells should have enough margins.<br />
Hard edges should be separated on UV.<br />

![Example of UVs for baking](img/bake-tutor-1/uvs-prepared.png)

*Example of mesh with UVs ready for baking.*

## Add image node to the object's material

Make sure that you have your mesh selected.<br />

![Add Image Shader Node](img/bake-tutor-1/shader-add-image-node.png)


In Shader Editor, choose **Add --- Texture --- Image Texture**<br />

![New Image](img/bake-tutor-1/image-new.png)

In that node, click **New**

![New Image Settings](img/bake-tutor-1/image-settings.png)


In this window, choose the **Name** of your map, **Width** and **Height**.<br />
**Alpha** is not needed for Normal Map, so we can turn it off.<br />
After that, click OK

![Color Space](img/bake-tutor-1/image-non-color.png)

It's very important to set **Color Space** to **Non-Color**. Now we're done with the image.

![Final Shader](img/bake-tutor-1/image-final-shader.png)

Final shader looks like this. You don't need to connect the image node anywhere right now.<br />
We recommend to bake with the Preview Node on. If it's not present in your material, you can add it by using [**Preview Mat Override**](npanel.md#2-preview-material-override-toggle) button in Zen BBQ N-Panel.



## Baking Settings

Make sure you have your object selected.<br />

![Quality Settings High](img/bake-tutor-1/npanel-high.png)

Make sure you have Quality setting in the N-Panel set to High.
![Bake Settings](img/bake-tutor-1/bake-settings.png)

In **Render Properties** Tab:<br />
In **Bake Accordion** change:

- **Bake Type**: Normal
- **Selected to Active**: Off
- **Margin Type**: Extend

In **Render Accordion** I prefer to choose **Time Limit**, for example, 15 minutes. The more time you set, the better quality you will get. 5-15 minutes are OK to render a draft variant. Of course, it depends on your computer's power, image resolution, mesh complexity, et cetera.

## Bake

![Start Baking](img/bake-tutor-1/bake-start.png)

When you're set, click **Bake** and wait till it's done.

## Viewing the result

In **Shader Editor**:

![Remove Preview Node](img/bake-tutor-1/remove-preview-node.png)

- Remove the Preview Node (Manually or by using [**Preview Mat Override**](npanel.md#2-preview-material-override-toggle) button in Zen BBQ N-Panel.

![Add a Normal Map Node](img/bake-tutor-1/add-normal-map-node.png)

- Add a Normal Map node

![Connect Nodes](img/bake-tutor-1/connect-nodes.png)

- Connect output of it to Normal input of your surface, and your Image Node Color output to the Color input of the Normal Map node.

![Surface Settings](img/bake-tutor-1/surface-settings.png)

- We're mostly done. Now adjust your material if you want to. I set somewhat grey-ish **Base Color** and **Metallic** to 1 for better viewing the result.

![Cycles to Eevee](img/bake-tutor-1/cycles-to-eevee.png)
![Eevee result](img/bake-tutor-1/eevee.png)

- Now we can choose Eevee render to see the result

!!! Notice
    Longer baking time and higher normal map resolution will give less artifacts.


## Exporting Normal Map


![Image Editor](img/bake-tutor-1/image-editor-choose.png)

In **Image Editor**, open your baked Normal Map.

![Save As](img/bake-tutor-1/image-editor-save-as.png)

And now you can choose **Image** --- **Save As...** it for usage outside Blender.

![Result](img/bake-tutor-1/MyBakedNormal.png)

*The result baked Normal Map*