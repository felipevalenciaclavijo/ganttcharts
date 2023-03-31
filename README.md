# Gantt Charts in R's ggplot2

This project is for creating a template to make Gantt Charts in ggplot2 using the speficied format and variables labelling. This project is mostly based on [Creating a pretty Gantt chart with ggplot2](https://stats.andrewheiss.com/misc/gantt.html) by Andrew Heiss. I added my chart customization preferences on top of it.

__It's important to have the CSV dataset organized with the same variables like the following:__

![Example](example_datasource.png)

__*IMPORTANT NOTES:__
+ If you have more variables in your dataset, you might need to `select()` only the four needed or adjust the `gather()` function to ignore the extra variables. 
+ If your dates are formatted differently, you'll need to adjust the `lubridate` functions to match your date formats. This is fairly simple, look at the [documentation](https://lubridate.tidyverse.org/reference/ymd.html).
+ If you would like to reduce the characters displayed use `substr()` to get the number of characters you want and `paste0("...")`.

![Gantt Chart Example](timeline_TestData.png)
