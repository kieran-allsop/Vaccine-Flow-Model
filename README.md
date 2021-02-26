# Vaccine-Flow-Model

Vaccine-Flow-Model contains R code in a markdown file that replicates all simulations and calculations in the AEI Economic Perspectives paper [Modeling Protection from COVID-19 Based on Vaccine Supply and Administration Rates](https://www.aei.org/research-products/report/modeling-protection-from-covid-19-based-on-vaccine-supply-and-administration-rates/), written by [Kieran Allsop](https://www.aei.org/profile/kieran-allsop/), [James C. Capretta](https://www.aei.org/profile/james-c-capretta/), and [Scott Ganz](https://www.aei.org/profile/scott-c-ganz/).

## Overview

The markdown file [vaccine_flow_replication_file.rmd](https://github.com/kieran-allsop/Vaccine-Flow-Model/blob/main/vaccine_flow_replication_file.Rmd) makes it easy to reproduce all of the calculations in the paper [Modeling Protection from COVID-19 Based on Vaccine Supply and Administration Rates](https://www.aei.org/research-products/report/modeling-protection-from-covid-19-based-on-vaccine-supply-and-administration-rates/) released February 24th 2021. In the paper Kieran Allsop, James C. Capretta, and Scott Ganz model the rollout of COVID-19 vaccines in the US under different scenarios. Parameters of the model include deliveries, administration capacity, number of doses required by individuals of each vaccine candidate, and available stock. The authors model the available stock over time under three different capacity scenarios where the ceiling for doses administered per day is either 2.5 million, 3 million, or 3.5 million. Based on stock, deliveries, and capacity, the authors also model the progression of population protection under the same scenarios. In a second analysis, the Johnson & Johnson candidate is also considered and comparing the two analyses show the effects that the new candidate will have on the population protection timeline.

## How to use Vaccine-Flow-Model

View the code in [vaccine_flow_replication_file.rmd](https://github.com/kieran-allsop/Vaccine-Flow-Model/blob/main/vaccine_flow_replication_file.Rmd). This markdown file contains all of the code and produces the graphs given in the report. Running each section in order will produce the desired simulations. There are sections for initializing the data, setting up future delivery schedules, setting up capacity constraints, creating functions to the run the model, runnng the model, and producing the graphs. The file [vaccine_flow_replication_file.html](https://github.com/kieran-allsop/Vaccine-Flow-Model/blob/main/vaccine_flow_replication_file.html) provides the same code and descriptions but in an easier to read format in a html compiler.

## Data Sources Used in Code

* [CDC COVID-19 tracker](https://covid.cdc.gov/covid-data-tracker/#vaccinations)
* [Moderna Shipping Schedule - CDC](https://data.cdc.gov/Vaccinations/COVID-19-Vaccine-Distribution-Allocations-by-Juris/b7pe-5nws)
* [Pfizer Shipping Schedule - CDC](https://data.cdc.gov/Vaccinations/COVID-19-Vaccine-Distribution-Allocations-by-Juris/saz5-9hgg)
* [Our World in data](https://github.com/owid/covid-19-data/tree/master/public/data/vaccinations) *(used to calculate rate of capacity growth)*
* [Bloomberg COVID-19 Vaccine Tracker](https://www.bloomberg.com/graphics/covid-vaccine-tracker-global-distribution/)
