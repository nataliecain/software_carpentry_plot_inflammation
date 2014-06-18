#Natalie Cain 06/16/14
#Software Carpentry final task

```r
setwd("/Users/natalie/Desktop/SWC/")
gDat <- read.delim("data/gapminder.txt")

#load libraries
require(ggplot2)
require(reshape2)

aus <- subset(gDat, country=="Australia")
can <- subset(gDat, country=="Canada")
u.s <- subset(gDat, country=="United States")

ggplot(aus, aes(year, gdpPercap))+geom_point()
```

![plot of chunk unnamed-chunk-1](figure/unnamed-chunk-1.png) 
