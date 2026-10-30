# AI and Deskilling — Registered Report

Public research materials for the registered report “Does LLM Assistance Lead to Deskilling?
A Longitudinal Multi-Domain Test”.

## Repository guide

- **[Pilot Study](Pilot%20Study/)**
  - [R Markdown source](Pilot%20Study/Analysis_Pilot_Public.Rmd) and [HTML report](Pilot%20Study/Analysis_Pilot_Public.html).
  - `data/`: four CSV files containing participant records, item-level test responses, AI consultation records, and anonymised age aggregates for the primary sample.
  - `output/figures/`: exported figures in PNG and PDF formats.
- **[Sample Size Calculation](Sample%20Size%20Calculation/)** — Sample-size planning, sensitivity analyses, attrition assumptions, and recruitment cost estimates.
  - [R Markdown source](Sample%20Size%20Calculation/SampleSize_RegisteredReport.Rmd) and [HTML report](Sample%20Size%20Calculation/SampleSize_RegisteredReport.html).

## Getting started

Open the HTML reports in a browser.

To rerun an analysis, open `Deskilling.Rproj` in RStudio. Use R 4.6.0 and restore the packages recorded in `renv.lock` from the repository root:

```r
install.packages("renv", repos = "https://cloud.r-project.org") # once
renv::restore()
renv::load()
```

Open the `.Rmd` file and knit to HTML. To run chunks interactively, set the working directory to the folder containing that file.

Rendering requires Pandoc (included with RStudio); exporting PDF figures also requires an R installation with Cairo support.
