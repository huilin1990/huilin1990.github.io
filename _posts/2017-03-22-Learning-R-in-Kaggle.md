---
layout: post
title: Learning R in Kaggle
date: 2017-03-22 12:35
tags: R
---
I'm learning data analysis and explore in R following the tutorial posted in [Kaggle](https://www.kaggle.com/mrisdal/titanic/exploring-survival-on-the-titanic)

Here are some sentences I found it useful.

`train <- read.csv('../input/train.csv', stringsAsFactors = F)`

This is how to read csv files. Also, use `read.delim()`, `read.delim2()` to read txt file.[read documentation](https://stat.ethz.ch/R-manual/R-devel/library/utils/html/read.table.html)

`stringAsFactors` is a useful factor. Here we do not want to use the headers as factors.

`str(dataframe)` use this to check data. Also if you use R Studio, use `view(dataframe)` to check data.

To check dataframe, we can also use `tbl_df` function.

```
full_df <- tbl_df(full)
full_df
```
