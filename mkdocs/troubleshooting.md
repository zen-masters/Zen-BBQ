---
title: "Troubleshooting & FAQ"
description: "Solutions to common issues with Zen BBQ installation, viewport display, baking artifacts, and Live Boolean integration."
category: "Support"
tags: [zen-bbq, blender, troubleshooting, help, baking, cycles]
related_files: [installation.md, quickstart.md, subpanel_bevels.md, subpanel_tools.md, live_boolean.md]
---

# Troubleshooting & FAQ

This guide covers the most common questions and issues users encounter when using Zen BBQ.

---

## 1. Zen BBQ Tab is Missing in the N-Panel

If you have installed the addon but cannot find the **Zen BBQ** tab in the sidebar (N-Panel):

*   **Check Blender Version:** Zen BBQ 2.0+ utilizes the local extension architecture and requires **Blender 4.2 LTS or newer**. It will not function on older versions.
*   **Activation Check:** Go to `Edit -> Preferences -> Get Extensions`. Search for "Zen BBQ" and ensure the checkbox is enabled.
*   **Installation Method:** Ensure you followed the correct [Installation Guide](installation.md). We recommend the "Drag and Drop" method for simplicity.

> 💡 **Note:** If you are using an older version of Blender (e.g., 3.6 or 4.1), you must use the legacy Zen BBQ 1.x version instead.

---

## 2. Procedural Bevels are Not Visible in the Viewport

If you have assigned bevels but don't see any rounded edges on your model:

*   **Switch to Shader Mode:** Zen BBQ uses a dedicated display engine. Ensure you have selected the **Shader Mode** button (the middle one in the display switcher) in the **Bevels** subpanel.
*   **Render Engine:** Procedural bevels rely on the **Cycles Bevel Shader**. Ensure your Render Engine is set to **Cycles**. Zen BBQ will typically prompt you to switch, but you can check this manually in the `Render Properties` tab.
*   **Object Selection:** Zen BBQ uses a non-destructive material override. You must have at least one object selected for the display mode switcher to work.
*   **Shader Settings:** Check if **Shader Bevels Preview** is enabled in the Shader popover configuration.

> 💡 **Note:** You must use the dedicated **Shader** button to see procedural results and the **Material** button to return to your original shaders.

---

## 3. Artifacts or Bleeding During Map Baking

If your baked Normal, AO, or Curvature maps show dark spots, bleeding, or projection artifacts where parts of the mesh intersect:

*   **Use the Explode System:** Multi-part meshes often cause projection issues during baking. Use the **BBQ Explode System** found in the **Tools Panel**.
*   **How to fix:**
    1.  Select your object and navigate to the **Tools** subpanel.
    2.  Click **Add Explode**. This will apply a procedural displacement to separate the mesh parts (Loose Parts) in 3D space.
    3.  Perform your bake while the mesh is "exploded".
    4.  Disable or remove the Explode modifier after baking is complete.

> 💡 **Note:** For the best results with the Explode System, it is highly recommended to use an **Empty** as the **Explosion Center** to precisely control the direction of part separation.

---

## 4. Live Boolean Cuts are Missing Bevels

If you are using a non-destructive Boolean workflow and the new cuts do not automatically receive a bevel:

*   **Check Default Radius:** Zen BBQ needs a fallback value for new edges. Go to the **Tools** subpanel and ensure a **Default Radius** is set.
*   **Configuration:** Click **Set Default Radius** and enter your desired value (e.g., 2mm). All subsequent boolean operations on the selected objects will now inherit this radius for their intersection edges.
*   **Modifier Order:** If you are using the **Node VC Mask** for export, ensure the modifier is at the very bottom of your stack to capture all dynamic boolean intersections.

> 💡 **Note:** You can adjust the global fallback radius at any time, and all non-destructive boolean cuts on the object will update their bevel widths accordingly.

If you have any question, please let us know:
![Discord](img/icons/services/discord-16.png) [**Discord**](https://discord.gg/wGpFeME)

---

[![Gumroad](img/icons/services/gumroad-16.png) **Gumroad**](https://sergeytyapkin.gumroad.com/l/zenbbq) | [![Superhive](img/icons/services/superhive-16.png) **Superhive**](https://blendermarket.com/products/zen-bbq) | [![Discord](img/icons/services/discord-16.png) **Discord**](https://discord.gg/wGpFeME)