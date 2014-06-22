---
title       : Body Mass Index Calculator
subtitle    : BMI Calculator
author      : Deano24 (Rohan Malcolm)
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
---

## App Summary
1. The body mass index (BMI) is a measure of relative weight based on an individual's mass and height.
2. Accuratley calculates the BMI of a person using the basic units of society.
3. Does automatic conversions so you don't have to.
4. BMI stands for Body Mass Index which is a ratio between weight and height.

---

## Why this App

I built this app because obesity, malnutrition and other health issues are directly related to a persons BMI. Several reasons exist as to why a person becomes large, obese, skinny and so on; some common reasons are over eating, wrong eating patterns, etc. Over all a large amount is down to poor eating habits and health habits.
Some individuals do not know that they are currently at a health risk due to their body size and I hope that this application can allow persons to quickly and efficiently calculate their BMI and use this information to make better health related choices.

---

## Data Interpretation

1. The system uses the calculation below to get the BMI $$(\frac{weight}{height^2})*703$$
2. For standardization in the formula the height is converted from the chosen unit to inches and weight to pounds.
3. Converting feet to inches is done by $$feet*12$$
4. Converting ounce to pounds is done by $$ounce/16$$
5. Converting ounce to pounds is done by $$stone*14$$

---

## What is BMI and Why is BMI Important?

BMI is a tool for finding relation between body size and body fat. Carrying excess body fat, not muscle, puts you at greater risk for health problems such as heart disease, cancer, diabetes and stroke. 

```r
    bmi <- (97/(58*58))*703
    if(bmi<18.5){
      "You are under weight"
    }else if(bmi>18.5 && bmi<24.9){
      "You have an ideal weight"
    }else if(bmi>24.9 && bmi<29.9){
      "You are over weight"
    }else{
      "You are obese"
    }
```

```
## [1] "You have an ideal weight"
```
Enjoy :) the system it can be found here [ShinyApps](https://deano24.shinyapps.io/CourseProject/) 
