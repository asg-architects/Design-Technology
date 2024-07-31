# Revit Automations - PyRevit

## Problem Statement
We perform too many tedious and repeative tasks in Revit that can consume a large amount of time.

## Thesis
By creating a collection of automation scripts, we can reduce the time spent on these laborious tasks.

## Summary
We created a collection of pyRevit Scripts that can be automatically loaded into Revit for use by the whole firm.

## Application
- **Wall Fixer**: You know that issue when you go to print your partition schedule and all of the tables are super whacked out? That's because our partitions have special values that define whether they have an acoustical or fire rating value; and by default, those values are set to *null*. Not 0 or no, but null, and that creates a whole lot of unpleasantness. This problem has been resolved in later versions of Revit, but if you are working on anything before Revit 2024, just click the Wall Fixer button and it will fix you right up. This button will read through all the partitions + walls in your model (anything not set to the **Reference Only** phase) and set Acoustical and Smoke values not set to Yes to be No and it will set any Fire Rating value less then .5 to 0. It's important to note that this button does not fix the overall issue of newly modeled partitions and walls having null values, it only sets values of elements already modeled. So, you will need to click the button prior to printing to ensure you are capturing all modeled elements. 
- **Graphic Scales**: This is not a new script, just an update to make it more usable. In the update, it will now auto-import the required families and shared parameters needed for the graphic scale. So all you have to do to get dynamic graphic scales added to your sheet viewports is click the "Add Graphic Scale" button and select the sheets, the script does the rest. Refresher for anyone who hasn't used this script before (which I think is everyone). How this works is, it adds the graphic scale to the view title on your viewport that way the scale is always at the same place, even if you move a view on the sheet. There are a set of pre-defined view types that will get the graphic scale viewport, so you just need to select which sheets you want the graphic scale applied to. Unfortunately, the built-in scale parameter for a view is not accessible by the family, so we had to create our own writable scale value, so after you place the graphic scales, you will need to push the "Set View Scale Value" button, this will take care of the rest. Final note, the graphic scale pattern is static and works best with even numbered scales (i.e. 1/4", 1/8") I am working on a dynamic model for odd scales (i.e. 3/32"), but this is a little lower on my list. 


## Links

- [Post on the Square](https://thesquare.ayerssaintgross.com/_layouts/15/Updates/ViewPost.aspx?ItemID=36145)

## Conclusion

![Image](./assets/pyRevit.jfif)