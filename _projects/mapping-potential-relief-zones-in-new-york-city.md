---
layout: project-page
title: "Mapping Potential Relief Zones in New York City"
linkname: mapping-potential-relief-zones-in-new-york-city
author: "Nicholas Arvanitis"
tagline: "Public facility access has been an ongoing challenge for New York City. As disasters become routine, these amenities are increasingly important."
location:
    - place: New York City, New York, USA
project-link:
    - href: <iframe width="100%" height="520" frameborder="0" src="https://thenewschool.carto.com/u/arvan536/builder/b3402d92-cd2a-457e-a020-dff9c26cd6cf/embed" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
    - href:  <blockquote class="imgur-embed-pub" lang="en" data-id="a/KvtsceP"><a href="//imgur.com/a/KvtsceP">View post on imgur.com</a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>
tags:
    - tag: climate resilience
    - tag:  homelessness
    - tag:  parks
    - tag:  infrastructure
    - tag:  plumbing
    - tag:  water
    - tag:  restrooms
    - tag:  community fridges
    - tag:  street furniture
    - tag:  community gardens
thumbnail-path: img/mapping-potential-relief-zones-in-new-york-city/FTFpOB3.jpg
img-folder: ../../img/mapping-potential-relief-zones-in-new-york-city/
timestamp: undefined
---
Public restroom access has been an ongoing challenge for New York City since the closure of many public facilities in the 1970’s. As a result of large amounts of public debt, the city was forced to rely on the private sector to provide similar amenities to the public. 

In the 1980’s homelessness began to emerge as a more prominent urban issue, partly in response to the divestment in public affairs. As public facilities, like restrooms and comfort stations began disappearing, this greatly impacted the homeless population leaving them without access to basic dignity in public.

In the present context, as disasters become routine, these amenities are increasingly important. The impact of COVID-19 further exposed this dilemma as a result of public restroom access in private spaces closing down as a result of public health measures. Furthermore, with increasingly worrisome climate events happening more regularly, public facilities have the unique potential to address issues relating to resiliency, equity and dignity to those in need. The equalizing potential of large scale disasters only makes relief infrastructure that much more necessary.

This project served as a geospatial analysis the city in order to find the best potential site to realize an assemblage of relief infrastructure. Firstly, I wanted to get a full picture of where all of the current street furniture managed by the Department of Transportation (DOT) is located across New York. Street furniture consists of bus shelters, newsstands, bike shelters and automatic public toilets (APT). I used custom html styling for each layer in order to build a hierarchy of information and created a custom base layer in mapbox in order to filter out information that was not particularly useful to the narrative.

<iframe width="100%" height="520" frameborder="0" src="https://thenewschool.carto.com/u/arvan536/builder/b3402d92-cd2a-457e-a020-dff9c26cd6cf/embed" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

APTs were initially the focus of my research, but after visiting the most popular site in Corona Plaza and speaking with the DOT, I realized that the initiative was a failing one and decided to focus elsewhere.

In order to gain a better understanding of where these relief zones could exist, I needed to build a map that could pin point the most ideal locations in the city to house these amenities. I decided to find all the parks within a short distance (500 feet) of transit stops as a starting point. Then I overlaid the 100 year flood plane estimate to see which of those parks would be most affected by climate disasters. Finally, I highlighted all the regions in accessible parks that were within a short distance to the flood plane, in order to locate the most ideal spaces for disaster relief infrastructure.

<a href="![]({{ page.img-folder }}SNTpWTt"><img) src="![]({{ page.img-folder }}SNTpWTt.jpg") title="source: imgur.com" /></a>

I noticed that Tompkins Square Park in Manhattan’s East Village could be exactly what I was looking for.

My next goal was to locate where the rest of the existing basic public amenities where located in this area. I decided to include community fridges, sprinklers, water taps, community gardens and of course, park restrooms.

<a href="![]({{ page.img-folder }}2jwBIPL"><img) src="![]({{ page.img-folder }}2jwBIPL.jpg") title="source: imgur.com" /></a>

This confirmed that Tompkins Square Park was a great potential site for creating a relief zone, since many important amenities are already present in the area.

Lastly, I decided to map out all of the 311 complaints about homeless encampments in parks in 2021. 
This would help reveal where homeless populations, the most vulnerable population, were congregating.

<a href="![]({{ page.img-folder }}1oMJ1ID"><img) src="![]({{ page.img-folder }}1oMJ1ID.jpg") title="source: imgur.com" /></a>
Once again, Tompkins Square Park lit up with 311 complaints, confirming a large presence of homeless encampments.