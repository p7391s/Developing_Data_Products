---
title       : Shiny Application and Reproducible Pitch
subtitle    : 
author      : ps7391
job         : 
framework   : revealjs        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## <span style="color:red; font-weight:bold">Developing Data Products</span>
## <span style="color:blue; font-weight:bold">Shiny Application and Reproducible Pitch</span>
### Display of Dependence of flavonoid content on alcohol content wines

ps7391

February 11, 2019

--- .class #id 

## <span style="color:green; font-weight:bold">Assignment</span>

Presentation must satisfy the following:

1. It must be done in Slidify or Rsudio Presenter
2. It must be 5 pages
3. It must be hosted on github or Rpubs
4. It must contained some embedded R code that gets run when slidifying the document

--- .class #id

## <span style="color:purple; font-weight:bold">Shiny Application</span>

The name of the application is "Display of Dependence of flavonoid content on alcohol content wines".

This app uses the dataset Wines. This dataset is part of the kohonen package.

This dataset provides various characteristics of wines.

Packages are used for interactivity in the application plotly and ggplot2.



You can download the shiny application for this repository and run it from you R-Studio using https://github.com/p7391s/Developing_Data_Products

---

## <span style="color:red; font-weight:bold">Instructions to run it</span>

Using the slider you choose the number of wines for which the dependence of the amount of alcohol on flavonoids will be displayed. The application shows the number of wines you have selected for selection.
Graphics made using the package ggplot2.


```r
    g <- ggplot(data, aes(alcohol, flavonoids)) +
      geom_point(color = "red")
    g
```


If in the application you mouse over a point on the graph, then the characteristics of the fault will be displayed thanks to the use of the graph package.

---

## <span style="color:salmon; font-weight:bold">Example plot from the application</span>


![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3-1.png)
### <span style="color:yellow; font-weight:bold">Thank you so much everyone</span>
