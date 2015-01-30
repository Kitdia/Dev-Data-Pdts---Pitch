---
title       : Investigating Central Limit Theorem with Exponential Distributions
subtitle    : 
author      : Kitdia
job         : Lecturer
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Problem

I want to demostrate the theory of Central Limit Theorem to my students.

However, doing it through R is kinda boring and might not interest them. 

--- .class #id 

## Proposed Solution

Create an interactive application so that 

- The results are intuitive enough for my students to understand

- They can explore it at home

- I can always re-use this application be it for future classes or for other lecturers' usage

--- .class #id

## Solution

Created an interactive Shiny Application. 

This application will investigate the distribution of averages of 40 exponentials, allowing students to choose the values for lambda and number of simulations and then returning the distribution of the simulated data.

Example
- Assume lambda is chosen to be = 0.2
- One simulated data will be produced through the r function: rexp(n,lambda)

```r
n=40
lambda=0.2
mean( rexp(n,lambda) )
```

```
## [1] 4.50442
```

The application and more info on it can be found at: https://kitdia.shinyapps.io/shiny2/ .

--- .class #id

## Thanks and feedback location

I hope this helps any lecturers with similar problem.

Please direct feedback to kitdia2903@gmail.com.

Thanks you for your time and feedback.


