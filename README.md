# Bayesian Sparse Factor Mixed Model

Work started during five-week rotation in Runcie Lab. 

## About

The data in markdowns is from Wolfgang Busch. Multiple Arabidopsis root traits from a 
high-throughput phenotyping pipeline for plants grown in various nutrient conditions.
This is written in R version 3.3.2

RootDataTransformed file goes through how the data files were combined an manipulated
prior to running BSFG.
Run_BSFG file goes through a run of BSFG with the data and subsequent analysis of the posterior.

### Prerequisites
The R devtools package needs to be installed to get BSFG.

``` {r prereq}
install.packages("devtools")

```
### Installing BSFG

The BSFG package can be installed from github

```{r install}
devtools::install_github("deruncie/SparseFactorMixedModel",subdir="BSFG",ref="one_general_model")

library("BSFG")
```

raw_data Directory contains root data and plant_id codes for the untransformed and log-transformed (T_ superscript) data



## Acknowledgments

* Dan Runcie
* Caryn Johansen
* Wolfgang Busch (for the data)


