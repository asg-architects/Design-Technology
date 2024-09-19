# Context Model Creation Automation

## Problem Statement
The existing process and workflows for creating and rendering compelling ariel fly-throughs is expensive and time-consuming

## Thesis
A new workflow that utilizes real-time renderings engines, 3D map tile, and repeatable interoperability between the Design Tools and the Visualization Tools will improve the viability of quality of the aerial narrative we wish to craft. Workflows for the importing of photometric Context Models eliminates the need for re-modeling context and increases the accurancy when handing off to the Viz team.

## Summary

Tools:

- GoogleMaps 3D Tiles API: As of May 2023, Google now provides an API to access the 3D tiles that feed the Google Earth and Google Maps Platform. The API is free at a low tier of usage but can cost money if usage limits are hit.
- Cesium: is a Middle-man tool that can dynamically load Google Maps Tiles in the web, Unity, Unreal, and Omniverse. This removes the complexity barrier of working with the Google Map Tile API directly.
- Placemaker: is a Middle-man tool that can statically load Google Maps Tiles in Revit and Sketchup. Placemaker also provides an interface to loading High Res Satelite Imagery, and Open Street Map Data.
- Forma: is a conceptual modelling tools that provides sparse but accruate terrian data, and GIS based pacels, 3D buildings, and roads. Models can be exported for use in other applications.

On the Visualization Side:

- Unreal engine provides a powerful engine for compelling lighting, realiistic textures, and rich entorage while allowing for real-time immersion, and fast media exports.
- Cesium with GoogleMaps Tiles provides an accurate 3D context reconstructed from aerial and satalite photography, removing the tedious and time-consuming task of modeling existing context.

## Application

Brown University - Jewelry District Study: This was the first use of Cesium in Unreal for Visualization Purposes.
University of Maryland, Baltimore - Grad Housing Study: Cesium, Unreal
Rice University - Michaels P3 Housing Proposal: Placemaker, Sketchup
University of Texas, Austin - Michaels P3 Housing Proposal: Placemaker, Sketchup
James Madison University - Nursing School Proposal: Placemaker, Sketchup

## Conclusion
We confirmed that we could re-use a similar setup from one project to the next to deliver appealling results in a time-efficient manner.

## Next Steps
- Continue re-use when requested.
- Explore how to leverage the framework for interactive deliverables.
