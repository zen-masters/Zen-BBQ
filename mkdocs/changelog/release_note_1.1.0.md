# Version 1.1.0

## **General**

- Added **Vertex Color Mask** creation for exporting bevel values to external applications.  
- Bug fixes.  
- Optimization.

## **Vertex Color**

- Added an operator to create a vertex color mask for exporting bevel values to Marmoset Toolbag.  
- Added a Geometry Nodes-based modifier for dynamically generating vertex color masks.  
- Added an operator to get the minimum and maximum bevel values from the current object.

## **Optimization**

- The **Use Scene Lights** render setting has been completely removed from automation and is now controlled manually by the user.  
- The **Preview Mat Override** option has been excluded from automation and will not activate if a bevel value is set for a "new" object.  
  You can enable automatic activation in the add-on preferences (Override material when assigning bevel).

## **Fixes**

- Fixed switching to Render Preview mode, where the viewport would always switch to Solid mode instead.  
- Fixed a bug that occurred after using the **Global Cleanup** operator, which caused the add-on to stop functioning.