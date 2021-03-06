
# rcmdcheck

> Run R CMD check from R and Capture Results

[![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
[![Linux Build Status](https://travis-ci.org/MangoTheCat/rcmdcheck.svg?branch=master)](https://travis-ci.org/MangoTheCat/rcmdcheck)
[![Windows Build status](https://ci.appveyor.com/api/projects/status/github/MangoTheCat/rcmdcheck?svg=true)](https://ci.appveyor.com/project/gaborcsardi/rcmdcheck)
[![](http://www.r-pkg.org/badges/version/rcmdcheck)](http://www.r-pkg.org/pkg/rcmdcheck)
[![CRAN RStudio mirror downloads](http://cranlogs.r-pkg.org/badges/rcmdcheck)](http://www.r-pkg.org/pkg/rcmdcheck)
[![Coverage Status](https://img.shields.io/codecov/c/github/MangoTheCat/rcmdcheck/master.svg)](https://codecov.io/github/MangoTheCat/rcmdcheck?branch=master)

Run R CMD check form R programatically, and capture the results of the
  individual checks.

## Installation

```r
devtools::install_github("mangothecat/rcmdcheck")
```

## Usage

```r
library(rcmdcheck)
rcmdcheck("path/to/R/package")
```

Call `rcmdcheck()` on a source R package `.tar.gz` file, or on a folder
containing your R package. Supply `quiet = FALSE` if you want to omit the
output. The result of the check is returned, in a list with elements
`errors`, `warnings`, and `notes`. Each element is a character vector,
and one element of the character vectors is a single failure.

![](/inst/screenshot.png)

## License

MIT © Mango Solutions
