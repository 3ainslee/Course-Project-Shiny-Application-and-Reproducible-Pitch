Shiny Application and Reproducible Pitch
========================================================
author: 
date: 
autosize: true

Summary Slide
========================================================

What we should expect in the upcoming slides

- Summary of the Data
- Plot of the Outliers
- Plot of the data
- Linear Model

Slide With Code
========================================================


```r
summary(cars)
```

```
     speed           dist       
 Min.   : 4.0   Min.   :  2.00  
 1st Qu.:12.0   1st Qu.: 26.00  
 Median :15.0   Median : 36.00  
 Mean   :15.4   Mean   : 42.98  
 3rd Qu.:19.0   3rd Qu.: 56.00  
 Max.   :25.0   Max.   :120.00  
```

```r
head(cars)
```

```
  speed dist
1     4    2
2     4   10
3     7    4
4     7   22
5     8   16
6     9   10
```

```r
par(mfrow=c(1, 2))  
boxplot(cars$speed, main="Speed", sub=paste("Outlier rows: ", boxplot.stats(cars$speed)$out))
```

![plot of chunk unnamed-chunk-1](Shiny Application and Reproducible Pitch-figure/unnamed-chunk-1-1.png)


Slide With Outliers
========================================================

![plot of chunk unnamed-chunk-2](Shiny Application and Reproducible Pitch-figure/unnamed-chunk-2-1.png)


Slide With Plot
========================================================

![plot of chunk unnamed-chunk-3](Shiny Application and Reproducible Pitch-figure/unnamed-chunk-3-1.png)![plot of chunk unnamed-chunk-3](Shiny Application and Reproducible Pitch-figure/unnamed-chunk-3-2.png)

Slide With Linear Model
========================================================


```

Call:
lm(formula = dist ~ speed, data = cars)

Coefficients:
(Intercept)        speed  
    -17.579        3.932  
```

```
[1] "The correlation is: "
```

```
[1] 0.8068949
```
