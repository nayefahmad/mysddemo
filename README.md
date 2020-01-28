
# mysddemo

<!-- badges: start -->
<!-- badges: end -->

The goal of mysddemo is to demo package dependencies issues. 

This is part of rstudio::conf 2020, on 2020-01-27. 

Reference: https://github.com/rstudio-conf-2020/build-tidy-tools/tree/master/notes

## Installation

You can install the released version of mysddemo from [CRAN](https://CRAN.R-project.org) with:

``` r
devtools::install_github("nayefahmad/mysddemo")
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
    * in the function defn itself, by writing `stats::var`. **Hadley: this is preferred, but can be very verbose. Also, you can't import an infix operator (e.g. %>%) using this method.**.  
* "import" means 2 diff things in the NAMESPACE file of the package and the DESCRIPTION file of the package. 
    * `use_package()` can be used to specify that we need to import packages in the DESCRIPTION file 
    
* When in interactive analysis mode, look into the {conflicted} package to resolve these namespace conflicts 


    



