---
title: Introduction to R
author: ["Madison"]
date: 2023-06-14 09:00:00 -0800
categories: ["R", "R_Getting Started"]
tags: ["R"]
---



R can be used as a generic calculator.


``` r
1 + 1
```

```
## [1] 2
```




``` r
2-3
```

```
## [1] -1
```




``` r
6 / 2
```

```
## [1] 3
```




``` r
3 * 4
```

```
## [1] 12
```



Since R is so widely used, there are many people who contribute to continuously improving and developing it. Without anything added, R is a base version. It can do basic calculations, but it requires extra efforts to do more complicated things. People have created extras or add-ons to help create shortcuts for more complicated specific tasks or functions. These 'add-ons' are called packages. Packages can be imported to use to help make things easier. For example, there is a large package in R called `tidyverse` that is very popular. 

First, packages must be installed, and then they have to be called. To install a package, use the command `install.packages('package_name')`. To call a package, use the command `library(package_name)`. This is one example below:


``` r
#install.packages('matlib')
library(matlib)
```

Once a package has been called, it does not need to be called again for the rest of this document. You can also import multiple packages within the same document. We will get into more useful packages later on!

For now, practice typing basic calculations into your R terminal to get used to the syntax, and see how easy it is to calculate things!
