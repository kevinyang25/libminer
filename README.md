
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer

<!-- badges: start -->

[![R-CMD-check](https://github.com/kevinyang25/libminer/workflows/R-CMD-check/badge.svg)](https://github.com/kevinyang25/libminer/actions)
[![R-CMD-check](https://github.com/kevinyang25/libminer/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/kevinyang25/libminer/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

The goal of libminer is to provide an overview of your R library setup.
It is a toy package created as part of a workshop and not meant for
serious use.

## Installation

You can install the released version of libminer from
[CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("libminer")
```

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("kevinyang25/libminer")
```

## Example

To get a count of installed packages in each of your libraries,
optionally with the total sizes, use `lib_summary()`.

``` r
library(libminer)
lib_summary()
#>                                                                                        Library
#> 1                               /Library/Frameworks/R.framework/Versions/3.6/Resources/library
#> 2 /private/var/folders/xv/m2p6kdr1183f09bbkfnygf8h0000gn/T/RtmpnPi51O/temp_libpath3ee226bd9ec7
#>   n_packages
#> 1        560
#> 2          1
#Specify sizes=TRUE
lib_summary(sizes=TRUE)
#>                                                                                        Library
#> 1                               /Library/Frameworks/R.framework/Versions/3.6/Resources/library
#> 2 /private/var/folders/xv/m2p6kdr1183f09bbkfnygf8h0000gn/T/RtmpnPi51O/temp_libpath3ee226bd9ec7
#>   n_packages   lib_size
#> 1        560 2025303169
#> 2          1      36854
```

What is special about using `README.Rmd` instead of just `README.md`?
You can include R chunks like so:

``` r
summary(cars)
#>      speed           dist       
#>  Min.   : 4.0   Min.   :  2.00  
#>  1st Qu.:12.0   1st Qu.: 26.00  
#>  Median :15.0   Median : 36.00  
#>  Mean   :15.4   Mean   : 42.98  
#>  3rd Qu.:19.0   3rd Qu.: 56.00  
#>  Max.   :25.0   Max.   :120.00
```

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this. You could also
use GitHub Actions to re-render `README.Rmd` every time you push. An
example workflow can be found here:
<https://github.com/r-lib/actions/tree/master/examples>.

You can also embed plots, for example:

<img src="man/figures/README-pressure-1.png" width="100%" />

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.
