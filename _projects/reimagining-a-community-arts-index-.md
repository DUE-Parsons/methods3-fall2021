---
layout: project-page
title: "Reimagining a Community Arts Index "
linkname: reimagining-a-community-arts-index-
author: "Meera Chakravarthy"
tagline: "My project looks to reimagine how we measure the impact of arts by zooming into the community arts level and adding a heavy spatial approach "
location:
    - place: New Orleans, Louisiana, United States of America
project-link:
    - href: https://thenewschool.carto.com/u/mchakravarthy/builder/d881099b-a0e2-4afb-8cea-f52f7a02c6dd/embed
tags:
    - tag: #communityarts #publichealth
thumbnail-path: img/reimagining-a-community-arts-index-/nfJ6Trw.png
img-folder: ../../img/reimagining-a-community-arts-index-/
timestamp: undefined
---
My research is focused on reimagining the role of collective culture and art delivery systems at the community level. Initially I found research that an index called the SMU Index exists to map vibrancy specifically in the US. However, I did not find this index was comprehensive enough to make the case that art spaces can affect the community and it’s relation to well-being. 

![]({{ page.img-folder }}iXzx8FS.png)
![]({{ page.img-folder }}DjQgQlI.png)


So, I set out to create my own community arts index. In order to build a community arts index, I first chose a geographic location that I thought was extremely vibrant and multicultural, but focused enough that it identifies strongly with art and small enough that it could be a test case in terms of data analysis. I chose New Orleans, Louisiana. 
![]({{ page.img-folder }}CGpbyEz.png)


When trying to collect data for an index, I initially created 4 main sections, employment, income, art spaces, and arts funding. I found shape files regarding arts spaces, found names of organizations for community arts funded organizations that I geocoded, found census data on arts employment, and was able to aggregate all of this to the census tract level. I also found data on artist income, but unfortunately I could not find it at the census tract level, so this data point could not be used. 

![]({{ page.img-folder }}hcR37Pb.png)

I got the employment data from Census.gov. It was actually in a category that lumped arts employment, recreation employment, and food service employment. Since I could not separate this data set just to get arts employment, I chose to still use it in my index but just weigh it at a lesser value than the other categories. 

![]({{ page.img-folder }}YFHLLCu.png)

I wanted to zoom into funding that goes directly to community based arts organizations so I found data on decentralized arts funding and community based arts funding and geocoded them using google maps. I created an excel file of the longitude and latitude coordinates and created a shapefile on QGIS. Then I did a count points polygon to understand the spread across census tracts. 

![]({{ page.img-folder }}22hJzyO.png)

![]({{ page.img-folder }}wpSHg2i.png)

![]({{ page.img-folder }}oNw55Dq.png)


I wanted to get a compilation of arts spaces, so I found shapefiles on literary nonprofits, libraries, museums, visual arts and crafts organizations, jazz houses, and live performance venues. I merged all of these files so they were in one shapefile and I did a counts point polygon to understand the spread across census tracts. I created categories based off what I found was low concentration of arts spaces versus high concentration of arts spaces. In the future, I would make this a buffer calculation. 

![]({{ page.img-folder }}acRPsRJ.png)

Finally, I wanted to include art spaces that were temporary. This includes festival grounds and parade routes. These were shapefiles. I simply did a binary analysis to see if they existed in a census tract or not. Because these were temporary art spaces, I wanted to weigh them less in my index. 

![]({{ page.img-folder }}xyPdF43.png)

I built my index by playing with the weights. I decided to give the following weights. In order to build the index, I had to create rule-based equations on QGIS so that the range of the particular variable in the index was aligned with the weight I gave that variable in my index. So for example if the index was out of 100 and arts funding was weighed at 35, I had to make sure my 4 categories in art spaces were equally distributed between 35. Ex: if a census tract had 1 art funded agency, it would be tagged at 8.75. If it had 2 -4 it would be tagged at 17.25 and so on.  I wrote equations like this for all 4 variables. 

![]({{ page.img-folder }}amWYsr4.png)

Once the components were built, I added them up to create my index. Then I mapped the index across census tracts. 

![]({{ page.img-folder }}YQd7GBf.png)

Finally, I found data on rates of depression by census tract from the CDC Places data. I decided to map this against my Arts Index. As you can see areas where the arts index is higher, there are generally lower rates and depression and vice versa. There seems to be a correlation between the data that I plan to further explore on R using correlation and regression analysis. 
Here you can see the components that make up the arts index mapped against the actual arts index. 

![]({{ page.img-folder }}2tQUWeq.png)

![]({{ page.img-folder }}tnq7Los.png)

![]({{ page.img-folder }}YQd7GBf.png)

My last step was to make this interactive on Carto. I decided to map all the points of the arts index and make them pop ups (in addition to the overall index score for that census tract), rather than just map the community arts index itself. I also create zoom CSS features that would allow various zoom levels, along with a base Map from Map Box that when zoomed in to 17, will show the buildings themselves. Since I was working with a gradient to showcase arts employment, I decided to just draw red lines around areas where depression rates were higher. In the future, I want to create another carto map that simply maps the consolidated index. I also want to improve my map by playing around with the weights of the index, perhaps create the categories of arts spaces/funding by a per population basis rather than categories I create on my own. Furthermore, I want to map other Places data such as chronic disease to show this data. 

![]({{ page.img-folder }}nfJ6Trw.png)
