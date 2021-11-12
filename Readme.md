NHS-R Recommended packages
================

Below you will find packages recommended by members of the NHS-R
community. These have been grouped by the type of package and how it is
typically applied in data analysis.

In addition there are some links to useful scripts, websites and
resources for other languages at the end of the document.

If you would like to suggest a package that you use in your role in the
NHS. Please consider filling in [this
form](https://airtable.com/shr7xXh4KJpAKzvZ8) so we can add the resource
to the page.  
Alternatively join the [NHS-R slack channel](nhsrcommunity.slack.com)
and add your recommendation as a post in the packages channel.

## Data visualisation

### ddplot

Create D3 based SVG graphics using a simple R Api

[GitHub url](https://feddelegrand7.github.io/ddplot/)

### runcharter

Plots multiple run charts, finds successive signals of improvement, and
revises medians when each signal occurs. Finds runs above, below, or on
both sides of the median, and returns a plot and a data.table
summarising original medians and any revisions, for all groups within
the supplied data.

[GitHub url](https://github.com/johnmackintosh/runcharter)

### simplevis

simplevis is a package of ggplot2 and leaflet wrapper functions that
aims to make visualisation easier with less brainpower required.

[GitHub url](https://statisticsnz.github.io/simplevis)

------------------------------------------------------------------------

## Data wrangling

### NHS-MSDS-pipeline

Automatically download, join, and clean the NHS Digital Maternity
Services Monthly Statistics data (MSMS), which is derived from the
Maternity Services Data Set (MSDS). When new information is released by
NHS Digital, re-running the scripts will add the new information to your
downloaded data, allowing analysis on the full dataset.

[GitHub url](https://github.com/ThomUK/NHS-MSDS-pipeline)

### numberwang

numberwang will convert floating point numbers (and integers) to their
word representations, and vice versa.

The key differentiator of this package, compared to {nombre}, is that it
supports decimal representations by listing individual decimal digits.

[GitHub url](https://github.com/coolbutuseless/numberwang)

### padr

padr is an R package that assists with preparing time series data. It
provides two main functions that will quickly get the data in the format
you want. When data is observed on too low a level, thicken will add a
column of a higher interval to the data frame, after which the user can
apply the appropriate aggregation. When there are missing records for
time points where observations were absent, pad will automatically
insert these records. A number of fill\_ functions help to subsequently
fill the missing values.

[GitHub url](https://github.com/EdwinTh/padr)

### widyr

Encapsulates the pattern of untidying data into a wide matrix,
performing some processing, then turning it back into a tidy form. This
is useful for several operations such as co-occurrence counts,
correlations, or clustering that are mathematically convenient on wide
matrices.

[GitHub url](https://github.com/dgrtwo/widyr)

------------------------------------------------------------------------

## Database

### dm

dm bridges the gap in the data pipeline between individual data frames
and relational databases. It’s a grammar of joined tables that provides
a consistent set of verbs for consuming, creating, and deploying
relational data models. For individual researchers, it broadens the
scope of datasets they can work with and how they work with them. For
organizations, it enables teams to quickly and efficiently create and
share large, complex datasets.

dm objects encapsulate relational data models constructed from local
data frames or lazy tables connected to an RDBMS. dm objects support the
full suite of dplyr data manipulation verbs along with additional
methods for constructing and verifying relational data models, including
key selection, key creation, and rigorous constraint checking. Once a
data model is complete, dm provides methods for deploying it to an
RDBMS. This allows it to scale from datasets that fit in memory to
databases with billions of rows.

[GitHub url](https://github.com/cynkra/dm)

------------------------------------------------------------------------

## Hospital Coding

### ICD

Calculate comorbidities, medical risk scores, and work very quickly and
precisely with ICD-9 and ICD-10 codes. This package enables a work flow
from raw tables of ICD codes in hospital databases to comorbidities.
ICD-9 and ICD-10 comorbidity mappings from Quan (Deyo and Elixhauser
versions), Elixhauser and AHRQ included. Common ambiguities and code
formats are handled. Comorbidity computation includes Hierarchical
Condition Codes, and an implementation of AHRQ Clinical Classifications.
Risk scores include those of Charlson and van Walraven. US Clinical
Modification, Word Health Organization, Belgian and French ICD-10 codes
are supported, most of which are downloaded on demand.

[GitHub url](https://github.com/jackwasey/icd)

### Rdiagnosislist

This is an R package for using the SNOMED CT hierarchy and manipulating
lists of SNOMED CT codes.

It includes functions for loading a SNOMED CT distribution into an R
environment, searching for concepts by regular expression search,
finding attributes of concepts, navigating the hierarchy, and handling
lists of SNOMED CT concepts.

[GitHub url](https://github.com/anoopshah/Rdiagnosislist)

### robson10classifier

The main function implemented so far is tgcs_classify(). It takes as an
input a data frame containing a minimum of 6 columns, one for each of
the obstetric variables that are used to classify the Robson Groups.
Each row in the data frame represents a birth. The function returns the
same data frame, with an additional column for Robson_Classification.
This can be a number from 1 to 10, or in the case that data required for
classification was missing, “Unclassifiable”.

[GitHub url](https://github.com/ThomUK/robson10classifier)

------------------------------------------------------------------------

## Modelling

### performance

Test if your model is a good model!

A crucial aspect when building regression models is to evaluate the
quality of modelfit. It is important to investigate how well models fit
to the data and which fit indices to report. Functions to create
diagnostic plots or to compute fit measures do exist, however, mostly
spread over different packages. There is no unique and consistent
approach to assess the model quality for different kind of models.

The primary goal of the performance package is to fill this gap and to
provide utilities for computing indices of model quality and goodness of
fit. These include measures like r-squared (R2), root mean squared error
(RMSE) or intraclass correlation coefficient (ICC) , but also functions
to check (mixed) models for overdispersion, zero-inflation, convergence
or singularity.

[GitHub url](https://easystats.github.io/performance/)

------------------------------------------------------------------------

## Reproducibility

### targets

The targets package is a Make-like pipeline toolkit for Statistics and
data science in R. With targets, you can maintain a reproducible
workflow without repeating yourself. targets learns how your pipeline
fits together, skips costly runtime for tasks that are already up to
date, runs only the necessary computation, supports implicit parallel
computing, abstracts files as R objects, and shows tangible evidence
that the results match the underlying code and data.

[GitHub url](https://docs.ropensci.org/targets/)

------------------------------------------------------------------------

## External data resource

### Deprivare

This provides code and data for indices of deprivation, initially
supporting the UK.

We know socio-economic deprivation has a significant effect on health
outcomes.

This repository provides a simple microservice, embeddable library and
command-line tools to allow other software to make use of deprivation
indices in the UK

[GitHub url](https://github.com/wardle/deprivare)

### LSOA POP

An R data package with Lower layer Super Output Area (LSOA) population
estimates and Indices of Multiple Deprivation (IMD) for England

[GitHub url](https://nhs-r-community.github.io/LSOApop/)

### medicaldata

This is a data package with 15 medical datasets for teaching
Reproducible Medical Research with R. The link to the pkgdown reference
website for {medicaldata} is here and in the links at the right. This
package will be useful for anyone teaching R to medical professionals,
including doctors, nurses, trainees, and students.

[GitHub url](https://github.com/higgi13425/medicaldata/)

### MHDS-pipeline

This is a data processing pipeline for the NHS Mental Health Services
Data Set

[GitHub url](https://github.com/sg-peytrignet/MHSDS-pipeline)

### RCPCH - Digital growth charts server

An API server and suite of tools which calculates growth centiles and
other growth related data for children. This is the basis of the RCPCH
Digital Growth Charts API.

Built with FastAPI in Python.

[GitHub url](https://dev.rcpch.ac.uk/)

------------------------------------------------------------------------

## R Development

### dbcooper

The dbcooper package turns a database connection into a collection of
functions, handling logic for keeping track of connections and letting
you take advantage of autocompletion when exploring a database.

It’s especially helpful to use when authoring database-specific R
packages, for instance in an internal company package or one wrapping a
public data source.

[GitHub url](https://github.com/dgrtwo/dbcooper)

### devtoolbox

rstats package for creating a single report on your package’s usage
stats, dependency network, and #GitHub PR/issues summary!

[GitHub url](https://github.com/martinctc/devtoolbox)

### Material for forwards workshops

The repo hosts the materials for workshop on R package development. The
links within the repo take you to the presentation slides, which refer
to online materials for the exercises and further reference. All
material in this repo is CC-BY-NC-SA.

[GitHub
url](https://github.com/forwards/workshops/tree/dc5b9fba5cdfbebc737a0a393b374a18378be122)

### riskmetric

riskmetric is a collection of risk metrics to evaluate the quality of R
packages.

This package is in experimentation. Final considerations about design
are being considered, but core concepts are considered final.

[GitHub url](https://github.com/pharmaR/riskmetric)

------------------------------------------------------------------------

## Rstudio Plugin

### remedy

Write quicker in markdown with {remedy}! Adds a plugin to. RStudio to
enable easier formatting of markdown

[GitHub url](https://github.com/ThinkR-open/remedy)

------------------------------------------------------------------------

## Rscript or function

### Package download tracker

A fuction that can be used to visualise package download metrics for
packages on CRAN

[GitHub
url](https://github.com/StatsGary/PackageTracker/blob/main/PackageTracker.R)

### RAG Quadrant icons

Tom wrote some code to make .png quadrant icons to summarise data
quality.

The icons are made using the {grid} package, and quite easy to change
around if you need something slightly different. Hopefully it might come
in handy to others here.

[GitHub url](https://github.com/ThomUK/STAR-quadrant-icon-maker)

------------------------------------------------------------------------

## Links

### Postcode deprivation finder

A web page where the Deprivation data for a postcode can be obtained

[GitHub url](NA)

------------------------------------------------------------------------

## Resources in other languages

### lux

Lux is a Python library that facilitate fast and easy data exploration
by automating the visualization and data analysis process. By simply
printing out a dataframe in a Jupyter notebook, Lux recommends a set of
visualizations highlighting interesting trends and patterns in the
dataset. Visualizations are displayed via an interactive widget that
enables users to quickly browse through large collections of
visualizations and make sense of their data.

[GitHub url](https://github.com/lux-org/lux)

### mermaid \[JAVASCRIPT\]

Mermaid lets you create diagrams and visualizations using text and code.

It is a Javascript based diagramming and charting tool that renders
Markdown-inspired text definitions to create and modify diagrams
dynamically.

If you are familiar with Markdown you should have no problem learning
Mermaid’s Syntax.

[GitHub url](http://mermaid-js.github.io/mermaid/)

### Tidypolars

tidypolars is a data frame library built on top of the blazingly fast
polars library that gives access to methods and functions familiar to R
tidyverse users.

[GitHub url](https://github.com/markfairbanks/tidypolars)
