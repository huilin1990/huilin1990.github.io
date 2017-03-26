---
layout: post
title: Learning R using Swirl
date: 2017-02-20 20:30
tags: R
---
# 用Swirl学习R语言，Learn R, in R

### Lesson: Regression Models Introduction

制图：plot(jitter(child,4) ~ parent,galton)

建立回归函数：使用函数`lm`(linear model)，例如：
```
regrline <- lm(child~parent, galton)
```
建立回归函数之后，使用`abline`(add straight lines to a plot)函数将回归函数在图表中画出，例如
```
abline(regrline, lwd = 3, col = "red")
#lwd = line width, col = line color
```
画出直线之后可以使用函数`summary`查看回归函数的各类参数包括残差， 系数，相关系数等等。

--------

### lesson: Getting and Cleaning Data
我们可以使用`read.csv`函数来导入数据。具体查看`?read.csv`，例子
```
#set a path to csv file
path2csv <-"E:/R-3.3.2/library/swirl/Courses/Getting_and_Cleaning_Data/Manipulating_Data_with_dplyr/2014-07-08.csv"

#use read.csv to read the csv file
mydf<-read.csv(path2csv,stringsAsFactors = FALSE)
#stringsAsFactors: logical: should character vectors be converted to factors?
```
使用`dim()`查看数据的行列情况
```
dim(mydf)
```
使用Dplyr包处理数据，首先`library(dplyr)`，然后使用`tbl_df()`(tibble)函数读取frame中的数据，这一步很重要，只有这样才能继续使用下面的函数和功能。
使用函数`rm("what_you_want_to_delete")`(remove)删除frame。
```
library(dplyr)
cran<-tbl_df(mydf)
rm("my_df")
```
五个最基础最常用的函数工具：`select()`, `filter()`, `arrange()`, `mutate()`, `summarize()`

-------

`select`函数可选取frame中的任意列，不用使用`$`符号。可以使用`:`，选取连续列，使用`-`删除不需要的列，例如
```
select(cran,country:r_arch)
select(cran, -(time:size))
```

-------

`filter`函数可以选取任意行
```
> filter(cran, package == "swirl")
> filter(cran,country == "IN", r_version <= "3.0.2") #, for AND
> filter(cran, country == "US" | country == "IN") #|for OR
> filter(cran, !is.na(r_version)) #
```
is.na()如果数据是空的，返回TRUE，反之FALSE

-------

`arrange`函数可以根据要求重新排列行的顺序。

```
arrange(cran, ip_id)
arrange(cran, desc(ip_id))
```

------
`mutate`函数可以用来增加一列派生变量。
```
> mutate(cran3, correct_size = size+1000)
```

-------

### Lesson2 Grouping and Chaining with dplyr
`summarize`是个很重要的函数。例如
```
by_package <- group_by(cran, package)
pack_sum <- summarize(by_package,
                      count = n(),
                      unique = n_distinct(ip_id),
                      countries = n_distinct(country),
                      avg_bytes = mean(size))

```
n()表示的是括号内的字段有多少不为空的数据，n_distinct表示括号内的字段有多少不重复的数据。这个函数是`length(unique(x))`的简化和快速版，更容易操作。

如果需要使用递进关系的函数，那么可以使用%>%连接符，可以连接不同函数。例如，
```
cran %>%
  select(ip_id, country, package, size) %>%
  mutate(size_mb = size / 2^20) %>%
  filter(size_mb <= 0.5) %>%
  arrange(desc(size_mb))
```
在上面的例子中，`select`函数需要用到`cran`数据框架，mutate函数需要用到`select`函数处理之后的数据框架，……以此类推。而在末尾的`%>%`连接符正好起到这样的作用。

---------

### Lesson Statistical Inference
本课程介绍三种R语言的绘图工具包：`plot`,`qplot`,`ggplot`。三种绘图包的能够和语法均不相同。
`plot`命令是R语言自带的绘图命令，绘图效果简单，适宜数据分析时绘图。
`qplot`命令是R语言初级绘图语言包，能够提供符合出版物标准的简单绘图。得到的图形大方美观。
```
qplot(hwy, displ, data = mpg)
```

qplot可调的参数有许多，如下展示

```

qplot(x, y, data=, color=, shape=, size=, alpha=, geom=, method=, formula=, facets=, xlim=, ylim= xlab=, ylab=, main=, sub=)

```
x, y, data, color, shape, size这些参数很容易理解。可以使用不同的变量实现变化。

alpha用于调节透明度。0就是全透明，1就是实心。

geom用于调节图表类型，有以下几个选项"point", "smooth", "boxplot", "line", "histogram", "density", "bar", "jitter".

point表示散点图

smooth做出拟合的曲线图

[boxplot](http://docs.ggplot2.org/0.9.3.1/geom_boxplot.html)做出股价图，此处不使用自定义的最高值，最低值和平均值，而是使用fill定义group，自动计算
```
qplot(year,averTLO, data = gt_sum, xlab = "Year", ylab = "Land&Ocean Avg Temp", geom = c("boxplot","jitter"),fill=decade)
```

![boxplot](/image/Land&Ocean Avg Temp vs year_boxplot_jitter.jpeg)

line做出折线图

[histogram](http://docs.ggplot2.org/0.9.3.1/geom_histogram.html)只针对单变量的柱状分布图，纵轴为count，横轴为该单变量。

[density](http://docs.ggplot2.org/0.9.3.1/geom_density.html)同样只针对单变量，画出该单变量的密度分布图。纵轴为density，横轴为该单变量。

[bar](http://docs.ggplot2.org/0.9.3.1/geom_bar.html)即为常规柱状分布图，定义两个变量,利用fill变量可以实现多种变化

```
qplot(factor(cyl), data=mtcars, geom="bar", fill=factor(gear))
```

![qplot](http://docs.ggplot2.org/0.9.3.1/geom_bar-18.png)


jitter则是在x轴上产生随机变量从而避免图形重叠带来的困扰。例如

```
p <- ggplot(mpg, aes(displ, hwy))
p + geom_point()
不用jitter散点图的效果
```

![points withou jitter](http://docs.ggplot2.org/0.9.3.1/geom_jitter-2.png)

```
p + geom_point(position = "jitter")
使用上jitter的效果
```
method和formula这两个选项是针对smooth这个选项而出现的。当smooth选项被调用，默认的拟合方法为loess。还有其他拟合方式允许被调用，如'lm':线性拟合，'gam':generalized additive models,"rlm": robust regression
```
For example, to add simple linear regression lines, you'd specify geom="smooth", method="lm", formula=y~x. Changing the formula to y~poly(x,2) would produce a quadratic fit. Note that the formula uses the letters x and y, not the names of the variables.

For method="gam", be sure to load the mgcv package. For method="rml", load the MASS package.
```
cited from [Quick-R](http://www.statmethods.net/advgraphs/ggplot2.html)

![jitter](http://docs.ggplot2.org/0.9.3.1/geom_jitter-4.png)

facets这个选项可以利用变量生成不同的分图，该选项的表达方式为：`facets=rowvar~colvar`，若rowvar或colvar不需要设置变量则用“.”代替。例如`facets = .~colvar`

利用coord_flip()可以将图表翻转

```
ggplot(diamonds, aes(color, fill=cut)) + geom_bar() + coord_flip()
```

![ggplot_bar](http://docs.ggplot2.org/0.9.3.1/geom_bar-22.png)

需要叠加不同类型的图表是使用c指令，e.g. `c("point", "smooth")`
```
qplot(year,averT, data = gt_sum, xlab = "Year", ylab = "Land Avg Temp", geom = c("point","smooth"))
```

![combine](/image/land avg temp vs year_point_smooth.jpeg)

xlim, ylim, xlab, ylab均容易理解
main,sub用于调节主副标题


`ggplot`采用图层式绘图方法，可根据自己的意图添加想要的图层，适合绘制复杂的大图。
下面是一个展示`ggplot`绘图语法的例子，其中`mpg`是`ggplot`自带的一个关于汽车品牌，性质的数据库。`hwy`和`displ`分别是`mpg`数据库中的字段，表示每加仑汽油行驶的里程数和汽车的排量。
```
>g<-ggplot(mpg, aes(hwy, displ))
>g+geom_points()+geom_smooth()
```
