# 🏗️ BuildingNodes

🏠 Tool for fast procedural building modeling | Blender add-on 🏠 

⏳ Work in progress ⏳

https://user-images.githubusercontent.com/28003269/140365097-63408046-33dc-4fd8-8cbf-4f52fe9dc973.mp4

## Features
- Cover vertical polygons (of base mesh) with wall panels.
- Using node editor for determining pattern of wall panels (facade style)
- Applying a facade style to as many objects as you wish
- Realtime applying facade style to an object in edit mode

## Roadmap
- Adjusting panels in building corners
- Supporting node groups
- Supporting geometry nodes
- Hipped roofs

## Limitations
- Using `Loop cut` tool with live update makes Blender to crush https://developer.blender.org/T67093
- Using `Edge crease` tool (Ctrl + E) with live update creases edges randomly
- Base mesh should consist only of quad polygons
- Animation is not supported

## Description
You can think about the add-on as a custom modifier based on node editor (similar to geometry nodes modifier).
Except that you won't be able to find it neither in list of modifiers nor in modifier stack because
custom modifiers are in [anti-features list](https://wiki.blender.org/wiki/Reference/AntiFeatures).
Instead, the main panel can be found in Property panel (N) of viewport editor.