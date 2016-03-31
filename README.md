# CatterPlots
Your source for cat themed plots.

<img src="https://github.com/Gibbsdavidl/CatterPlot/blob/master/examples/catplot_ex_6.png" width="300">

Go ahead, treat yourself! There's over 10 cat models now!

Well, exactly 11, actually. Eleven types of cats.

To install, either:
```
library(devtools)
install_github("Gibbsdavidl/CatterPlots")
```
Or git clone the repo and then install using:
```
R CMD INSTALL CatterPlots
```

In R:

```
library(CatterPlots)
x <- -10:10
y <- -x^2 + 10
purr <- catplot(xs=x, ys=y, cat=3, catcolor=c(0,1,1,1))
cats(purr, -x, -y, cat=4, catcolor=c(1,0,1,1))

# for more fun ...
meow <- multicat(xs=x, ys=y, cat=c(1,2,3), catcolor=list(c(1,1,0,1),c(0,1,1,1)), canvas=c(-0.1,1.1, -0.1, 1.1))
morecats(purr, x, 10*sin(x)+40, size=0.05, cat=c(4,5,6), catcolor=list(c(0,0,1,1),c(0,1,0,1)), type="line")

```
