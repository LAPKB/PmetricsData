
<!-- update README.md with devtools::build_readme() -->

# PmetricsData <a href="https://lapkb.github.io/Pmetrics/"><img src="man/figures/logo.png" align="right" height="139" alt="Pmetrics website" /></a>

<!-- badges: start -->
<!-- badges: end -->

PmetricsData provides datasets and examples which can be used with the
Pmetrics pharmacometric modeling and simulation package. They can also
be used in other relevant packages or applications.

Included are the following. Further details are included in the help for
each data item, e.g. `?NPex`.

### Pharmacokinetic data

- NPex - Output of a *nonparametric* model fit in a
  [PM_result](https://lapkb.github.io/Pmetrics/reference/PM_result.html).
- ITex - Output of a *parametric* model fit in a
  [PM_result](https://lapkb.github.io/Pmetrics/reference/PM_result.html).
- modEx - Model for absorption into central compartment in a
  [PM_model](https://lapkb.github.io/Pmetrics/reference/PM_model.html).
- model - The saved text file version of `modEx`.
- dataEx - Data based on oral rifapentine with frequent sampling in 20
  adults, all formatted as
  [PM_data](https://lapkb.github.io/Pmetrics/reference/PM_data.html).
- badData - Example of data with errors to show catch/highlight
  functions
- simEx - Simulation output using `NPex` and the first 4 subjects in a
  [PM_sim](https://lapkb.github.io/Pmetrics/reference/PM_sim.html).

### Other Data

- mic1 - Data frame with vancomycin minimum inhibitory concentration
  (MIC) and counts for methicillin-resistant *Staphylococccus aureus*
  (MRSA) obtained from EUCAST.
- growth - Data on height and weight percentiles by age and sex,
  from CDC. Can be used in the Pmetrics
  [qgrowth](https://lapkb.github.io/Pmetrics/reference/qgrowth.html)
  function.
- cdc_bmi, ger_bmi - Age and sex-specific BMI z-scores and percentiles
  from CDC or NHANES. Can be used in the Pmetrics
  [zbmi](https://lapkb.github.io/Pmetrics/reference/zBMI.html) function.
- locales - World languages and their iso693 two- and three-letter
  codes. Pmetrics uses these data to assist with location detection and
  proper date, decimal, and number separator formatting.

## Installation

You can install the development version of PmetricsData from
[GitHub](https://github.com/) with:

``` r
# install.packages("remotes")
remotes::install_github("LAPKB/PmetricsData")
```

## Example

``` r
library(PmetricsData)
NPex
#> <PM_result>
#>   Public:
#>     auc: function (type, ...) 
#>     clone: function (deep = FALSE) 
#>     cov: PM_cov, R6
#>     cycle: PM_cycle, R6
#>     data: PM_data, R6
#>     errfile: 
#>     final: NPAG, PM_final, R6
#>     initialize: function (out, quiet = TRUE) 
#>     ITdata: NULL
#>     load: function (...) 
#>     MM_opt: function (...) 
#>     model: PM_model_file, PM_model_list, PM_model, R6
#>     nca: function (...) 
#>     NPdata: NPAG, list
#>     op: PM_op, R6
#>     plot: function (type, ...) 
#>     pop: PM_pop, R6
#>     post: PM_post, R6
#>     save: function (run, file) 
#>     sim: function (...) 
#>     step: function (...) 
#>     success: TRUE
#>     summary: function (type, ...) 
#>     valid: PM_valid, R6
#>     validate: function (...)
```
