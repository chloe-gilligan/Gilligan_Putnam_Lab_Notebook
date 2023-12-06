---
layout: post
title: Histology Protocol
date: '2023-12-04'
categories: Protocols
tags: [Histology, ImageJ, Astrangia]
---

## Protocol for Analyzing Histology Slides

---

1) Open file from ImageJ

2) I tend to open a low quality image of the slide label and open one file in the highest quality possible for the first polyp.

3) Have spreadsheet ready with Coral ID, Collection Site, Treatment, Timepoint, File name (ex:AST-1035-TP4.vsi), Image name (ex: series #14), grid size (ex:11500 microns), scale, units of measurements (ex: microns), and finally the measurement desired from each stage.
	
- In my case, I did average size and abundance within each stage.

4) In tool bar select Analyze and then click set scale. Record the "distance in pixels" as the standard scale of measurements. This should be the same across files but make sure to check as you go through files.

5) Overlay a grid by selecting analyze in the toolbar, tools, and grid. Insert a grid that will allow you to guided through the file at an appropriate scale so you see the grid and stage one eggs. 

- 	Make note of the size of the grid.

6) In order to calculate relative abundance, I only totaled gamate numbers up to 50 which was an appropriate number given my species, so adjust accordingly. 

7) Starting on the grid at the top left-most point of where the polyp starts, go down the grid calculating the abundance of gamates, once the bottom of the polyp is reached on the first grid column, move one column to the right and continue counting. Continue moving one column right until 50 gamates are reached. Do this for each stage of gametogeneisis. 

- For example, I counted 50 stage one eggs and then repeated the process starting at the top left-most point for stage 2,3,4, and 5.
- I only recorded oocytes with full nucleus present in order to guarantee the stage being recorded.

8) In order to calculate average size per stage, restart the process starting at the top left most point of the coral on the grid.

9) In the ImageJ toolbar, select the bean-shaped button. This will allow you to trace nonregular shapes, creating an accurate trace of the size of gamate.

10) Using the same grid pattern go through for each stage, tracing 10 gamates. Take the average of the 10 traces which will be the average size of the respective stage. 

- In order to do this, take the tracing and select control/command M to take the measurement and physically average the 10 together.  

