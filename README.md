
# Introduction
This is my work from the Google Code-in task 'Draw a hexagon logo for an R package'. Below you can see the code with comments.

# Prerequisites
- R
- RStudio
- hexSticker
- ggplot2

# Code Description
The code below can be copied to R and executed as is.

```
library ("hexSticker")
library("ggplot2")
library("ACMEeqtl")
library("devtools")
if(!requireNamespace("devtools", quietly = TRUE))
  devtools::library("andreyshabalin/ACMEeqtl")

Logo1 = sticker(~plot(cars, cex=.6, cex.axis=.6, mgp=c(1,.4,1), xlab="1", ylab="2"),
        package="ACMEeqtl", p_size=20, s_x=.8, s_y=.6, s_width=1.4, s_height=1.2,
        filename="baseplotforACMEeqtl.png")

Logo2 = imgurl=system.file("C:\\Users\\srish\\Desktop\\10.jpg", package="hexsticker")
sticker("C:\\Users\\srish\\Desktop\\10.jpg", package="ACMEeqtl", p_size=20, s_x=1, s_y=.75, s_width=.6,
        filename="aa.jpg")

rbind(Logo1, Logo2)
write.csv(rbind)
```
# Logo 

![](aa.jpg)

# Author
- Srishti 
