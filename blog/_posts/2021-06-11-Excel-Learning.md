---
layout: post
title:  "Learning Excel for Data Analysts (And General Purposes)"
categories: Data_Analysis
truncated_preview: true
excerpt_separator: <!--more-->
---
Started going through the IBM data analyst program as mentioned. The first course is a data analytics basics which introduced the terms and concepts that are related to the field. Not too much to say about it, it's a mix of new information and things I've already read about before.

One thing I will say is that I'm not a fan of the way the material is shown. The presentation is pretty dry, pretty much felt like someone reading off a Powerpoint slide. The volume is also inconsistent between videos, I turn the volume up for one video and then have to turn it back down for the next one.

Anyways, the next part of the program is learning how to use Excel for data analysis. I'm already familiar with a lot of the more intermediate Excel concepts so I focused on learning how it is applied in a data analysis setting.

The course starts off by teaching me how to import data from text files. Then it explains how to use various Excel features to do basic data cleaning, such as:
- Spell check for misspellings
- Filter for empty rows/columns and delete
- Highlight duplicate data with conditional formatting
- Or just use the built-in Excel feature for deleting duplicate rows

Then it goes on to explain ways to make the data more consistent
- Changing casing with UPPER, LOWER, and PROPER
- Changing date format
- Removing whitespaces by find & replacing double spaces and using the TRIM function

And after that, just the usual Excel stuff of filtering, PivotTables, IF/IFS/SUMIFS/..., and VLOOKUP. I do like how they give a hands-on section with an example worksheet to practice the concept that they showed in the videos.

The next course is about data visualization and building dashboards. Creating charts in Excel is really simple, I find that it's more important to know what chart type to use. Nothing too notable about this section either, though one minor thing did stand out to me during the hands-on exercise.
<!--more-->

In one section of the exercise, it guides the reader through creating a line chart from a PivotTable using car sales data. It tells us to create this chart:

![Questionable table from IBM](/imgs/Excel1/IBMPivot.png "???")


Perhaps I'm missing something, but it makes absolutely no sense to use a line chart here. I guess they just wanted a simple way to demonstrate line charts with the same dataset. However, it bothered me that this was the example given so I modified the PivotTable a bit and made this:


![Japanese Manufacturer's Retention %s](/imgs/Excel1/MyPivot.png "Japanese quality")
![American Manufacturer's Retention %s](/imgs/Excel1/MyPivot2.png "Where did we go wrong?")

So it now displays the average retention % of models by latest launch date, filterable by manufacturer. The exercise had us filter by Japanese car manufacturers. So I figured I would compare the Japanese and American car manufacturers in the retention rate of their models over time by latest launch dates. Considering that only a few models release each month, these charts might not be that useful either. But hey, at least it has a historical element so using a line chart makes some sense. If I really wanted something to look into, it does appear that American manufacturers are on a slight downward trend when it comes to retention rates.

The last part of this course explains how to build dashboards using Excel. For some reason, I thought it would be at least a slightly tricky task. It turns out to be just pasting together and resizing charts into one area. Another questionable part did show up here. In the video, they put together the charts for the dashboard then starts talking about changing the style and color for a more consistent look which leads into this...

![A very green chart](/imgs/Excel1/IBMWhy.png "The human eye can see more shades of green than any other colors, but still...")

I suppose it looks nice, but that pie chart looks pretty hard to read when it uses various shades of green to represent different car models. I wonder if there's someone out there that followed this video too closely and presented a pie chart like this. Eh, it's not like the section was about style guidelines so I could give it a pass...wait a minute...

Anyways, the next section will be about analyzing and visualizing data with Python. Luckily I'm also already familiar with Python, so I can just jump straight into the applications.