# barrelr
[![RStudio][rstudio-badge]][rstudio-url]
[![R][r-badge]][r-url]
[![LinkedIn][linkedin-badge]][linkedin-url]

## About

#### barrelr is an R package for college baseball analytics.

This package includes the `is_barrel` function, which classifies batted-balls as barrels or not
based on their exit velocity and launch angle. 

A **barrel** is a batted-ball with a combination of exit velocity and launch angle that produces
an Expected Batting Average (xBA) of at least 0.500 and an Expected Slugging Percentage (xSLG) 
of 1.500 or greater. Barrels are a Statcast metric used to identify batted-balls with high 
offensive value.

> [!NOTE]
> `is_barrel` is trained on college baseball data. Consequently, its barrel classifications may not
align with [MLB](https://www.mlb.com/glossary/statcast/barrel) definitions or results.

## Installation

#### Install barrelr from GitHub using [`pak`](https://github.com/r-lib/pak#arrow_down-installation):

``` r
if (!requireNamespace('pak', quietly = TRUE)){
  install.packages('pak')
}
pak::pak("kylegilber/barrelr")
```

<!-- link definitions -->
[rstudio-badge]: https://img.shields.io/badge/RStudio-75AADB?style=for-the-badge&logo=RStudio&logoColor=white
[rstudio-url]: https://posit.co/downloads
[r-badge]: https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white
[r-url]: https://www.r-project.org/
[linkedin-badge]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url]: https://www.linkedin.com/in/kylegilbertpsu/
