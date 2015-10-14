---
title       : Car Mileage Prediction
subtitle    : A Shiny Application
author      : Mayur Narsude
job         : Data Science Factory
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Goal

1. Write a shiny application and supporting documentation
2. Deploy the application on Rstudio's shiny server

--- .class #id 

## Shiny Application
- The `mtcars` dataset is used to build a prediction model
- Very little attention is paid to the accuracy and efficiency of the model

The structure of `mtcars` dataset is as below

```
## 'data.frame':	32 obs. of  11 variables:
##  $ mpg : num  21 21 22.8 21.4 18.7 18.1 14.3 24.4 22.8 19.2 ...
##  $ cyl : num  6 6 4 6 8 6 8 4 4 6 ...
##  $ disp: num  160 160 108 258 360 ...
##  $ hp  : num  110 110 93 110 175 105 245 62 95 123 ...
##  $ drat: num  3.9 3.9 3.85 3.08 3.15 2.76 3.21 3.69 3.92 3.92 ...
##  $ wt  : num  2.62 2.88 2.32 3.21 3.44 ...
##  $ qsec: num  16.5 17 18.6 19.4 17 ...
##  $ vs  : num  0 0 1 1 0 1 0 1 1 1 ...
##  $ am  : num  1 1 1 0 0 0 0 0 0 0 ...
##  $ gear: num  4 4 4 3 3 3 3 4 4 4 ...
##  $ carb: num  4 4 1 1 2 1 4 2 2 4 ...
```

---

## Mileage Prediction App
- The dependent variable is `mpg` and the remaining variables are treated as predictor variables
- The entire `mtcars` data is used to train the `glm` model using `caret` package
- User of the app is expected to fill all the input fields and click "Go!" button
- Reactivity is controlled using `isolate` function in server.R
- A short and simple text is included in the shiny webpage as app documentation

---

## Summary
1. A shiny application for "Car's Mileage Prediction" is built using the `mtcars` dataset
2. The application is deployed successfully on Rstudio's shiny server.
The shiny webpage and corresponding code can be found at below URLs:

[Application](https://mayurnarsude.shinyapps.io/shiny)

[Code](https://github.com/mayurnarsude/developingDataProducts)







