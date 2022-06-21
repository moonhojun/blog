---
title: "20220621"
output:
  html_document:
    keep_md: true
date: '2022-06-21'
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

setwd("C:/Users/human/Desktop/R_edu/data")
mpg1 <- read.csv("mpg1.csv", stringsAsFactors = F)
str(mpg1)
mean(mtcars$mpg)
var(mtcars$mpg)
sd(mtcars$mpg)
sum(mtcars$mpg)
range(mtcars$mpg)

str(mpg1)
table(mpg1$trans)
table(mpg1$manufacturer)

table(mpg1$trans, mpg1$manufacturer)

a <- table(mpg1$trans)
prop.table(a)
