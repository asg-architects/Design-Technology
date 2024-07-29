# Space Visualization - UNC

## Problem Statement

When a client provides space-use data and floor-plan data in a low-intelligence data format like CAD and Excel, verifying the accuracity and integrity of university provided room data can be very challenging without proper visualization tools.

## Thesis

If we can create a repeatable correlation between floor-plans and space-use data, we can create powerful interactive dashboards that will help interogate, validate, and correct the data.

## Summary

the DT team explored multiple approaches to how we can correlate and then visualize client provided data.

Workflow 1:
1. Utilize Grasshopper to import CAD and Excel data, find associations in the data
2. Export geometry using layers to define data characteristics.
2. Use Rhino.Inside Revit to import the linework and Rooms into Revit
3. Create colored-plan views and schedules in Revit for export.

Workflow 2:
1. Utilize Grasshopper to import CAD and Excel data, find associations in the data.
2. Export the geometry with the associated Excel Data to Speckle.
3. Create a Power BI Dashboard that fetches the Speckle Model and slices the data based on different criteria?

## Application

UNC School of Public Health:
[Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNzJlMzViZTMtZTE4OC00YmZmLTkzMWQtODViZjU4YmZiMTZiIiwidCI6ImYwMDdiNTU2LWE4ZWItNDJkMi1hMDQ0LTMxNWM0YmQzNTk3NiIsImMiOjF9)

## Conclusion