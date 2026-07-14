---
title: "Zen BBQ Release Notes v1.2.0"
description: "Detailed changes in version 1.2.0: Update function, bevel statistics, and bug fixes."
category: "Changelog"
tags: [zen-bbq, blender, changelog, updates, statistics, optimization]
related_files: [changelog.md]
---

# Version 1.2.0

## **General**

- Added **Update** function that collect all bevel values and calculate maximum.
- Presets adjusted at scene level and normalized to standard Blender behaviour
- Bug fixes.  

## Enhancement
- Bevel statistics - how many objects have a corresponding bevel preset value

## Tools
- Replace bevel value
- Clear bevel values that are not present in the current preset

## **Fixes**

- **Render Preview** button freezes interface when a lot of objects are selected in the scene
- Edges highlight was not refreshed if mesh changed its hidden state
