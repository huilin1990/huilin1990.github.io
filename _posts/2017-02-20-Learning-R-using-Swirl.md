---
layout: post
title: Learning R using Swirl
date: 2017-02-20 20:30
tags: r
---
# 用Swirl学习R语言，Learn R, in R

>how to import data (read function)
>how to manipulate data wit dplyr

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
> mutate(cran3, temperature = mean(AvgTemp, na.rm = "TRUE")) #求平均值，把空值删除
> mutate(cran3, decade = trunc(year/10))#trunc函数取整， 一系列的函数还有floor(), round(),signif().
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
