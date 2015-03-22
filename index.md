---
title       : Pitch about my First Shiny app
subtitle    : To Finding Lineair Regression Line with dynamical Help
author      : S.R.Russel
job         : Coursera student
framework   : io2012 # {io2012, html5slides, shower, dzslides, ...}
highlighter : prettify  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Start with creating data ... 
We learn that Lineair Regression Line with certain values for intercept and slope has got the lowest standard deviation with data (Y,X), where Y is a set N response variables and X is a set N predictor. Let start with set number predictor variables to plot (Y,X) :
<img src="assets/fig/plot1-1.png" title="plot of chunk plot1" alt="plot of chunk plot1" style="display: block; margin: auto;" />
It keeps until we update (Y,X) with new random values. See next slide more about a line...

--- .class #id 

## ... and line
Before finding a Lineair Regression Line, our red Line is drawn with slope and intercept from sliders. With sliders we change values of slope and intercept, so we redraw red line. In the plot example, the line has got intercept=5 and slope=0.3.
<img src="assets/fig/unnamed-chunk-1-1.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" style="display: block; margin: auto;" />
At the Shiny app, we can read the standard deviation of our line below Plot window.
Be aware that the changing values are not smooth or that it is complex to adjust two values, so it may not easy to find lowest standard deviation.
Then go to next slide ...

--- .class #id 

## Help for searching lowest standard deviation
To find Lineair Regression Line, we have to find lowest standard deviation globally, not locally.
It is not easy to estimate it visually. So there is Help at the Shiny app: it "remembers" a lowest standard deviation we found so far and it draws corresponding grey line.
<img src="assets/fig/unnamed-chunk-2-1.png" title="plot of chunk unnamed-chunk-2" alt="plot of chunk unnamed-chunk-2" style="display: block; margin: auto;" />
So if we are sure there is no more minimum, then we can draw line by going back to last found lowest standard deviation. See next slide about a result...

--- .class #id 

## Confirm our result
When we are sure we create line with lowest value of standard deviation, then we compare our line with Linear Regression Line visually by checking 'Yes' to show Lineair Regression Line as green  line:
<img src="assets/fig/unnamed-chunk-3-1.png" title="plot of chunk unnamed-chunk-3" alt="plot of chunk unnamed-chunk-3" style="display: block; margin: auto;" />
We see we found the minimum locally, since grey line and green line are not positioned equally...
So keep on to try the [Shiny app](https://srrussel.shinyapps.io/project/). 
