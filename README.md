# Vaccine-Flow-Model

Vaccine-Flow-Model contains R code in a markdown file that replicates all simulations and calculations in the AEI Economic Perspectives paper [Modeling Protection from COVID-19 Based on Vaccine Supply and Administration Rates](), written by [Kieran Allsop](https://www.aei.org/profile/kieran-allsop/), [Jim Capretta](https://www.aei.org/profile/james-c-capretta/), and [Scott Ganz](https://www.aei.org/profile/scott-c-ganz/).

## Overview

The markdown file [vaccine_flow_replication_file.rmd]() makes it easy to reproduce all of the calculations in the paper [Modeling Protection from COVID-19 Based on Vaccine Supply and Administration Rates]() released February 24th 2021. In the paper Kieran Allsop, Jim Capretta, and Scott Ganz model the role out of COVID-19 vaccines in the US under differing scenarios. Parameters of the model include deliveries, administration capacity, number of doses required by individuals of each vaccine candidate, and available stock. The authors model the available stock over time under three different capacity scenarios where the ceiling for doses admisitered per day is either 2.5 million, 3 million, or 3.5 million. Based on stock, deliveries, and capacity, the authors also model the progression of population protection under the same scenarios. In a second analysis, the Johnson & Johnson candidate is also considered and comparing the two analyses show the effects that the new candidate will have on the population protection timeline.

## How to use Vaccine-Flow-Model

View the code in [vaccine_flow_replication_file.rmd](). This markdown file contains all of the code and produces the graphs given in the report. Running each section in order will produce the desired simulations. There are sections for initializing the data, setting up future delivery schedules, setting up capacity constraints, creating functions to the run the model, runnng the model, and producing the graphs. The file [vaccine_flow_replication_file.html]() provides the same code and descriptions but in an easier to read format in a html compiler.
