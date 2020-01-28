
# mysddemo

<!-- badges: start -->
<!-- badges: end -->

The goal of mysddemo is to ...

## Installation

You can install the released version of mysddemo from [CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("mysddemo")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(mysddemo)
## basic example code
```


## Notes 

* When you define a function using a function from another package (e.g. my_sd( ) is defined using stats::var()), you should be explicit about which package to find the other function in. Two ways to do this: 
    * in the Roxygen comment, like `@importFrom stats var`. First package name, then fn name 
    * in the function defn itself, by writing `stats::var` 


