---
title: Setup
---

For this lesson, you will be working in the R programming language and the 
RStudio development environment on the data analysis and sharing platform 
[CAVATICA](https://www.cavatica.org/).

## Setup

### Access CAVATICA

1. [Sign up for a free CAVATICA account](https://docs.cavatica.org/docs/sign-up-for-cavatica).

1. Request your free pilot fund cloud credits by 
[contacting CAVATICA support](https://docs.cavatica.org/docs/getting-started).

1. [Create a project](https://docs.cavatica.org/docs/quickstart#create-a-project). Give it a good descriptive name like `r-multiomics`.

1. For **Billing group**, select `Pilot Funds` if you have received free pilot 
fund cloud credits.

1. Under **Advanced settings**, change the default setting to `Allow network access`.
![](episodes/fig/block-network-access.png)

1. Copy the `env-rstudio-multiomics` project into your new project.

1. Run a 
[Data Studio analysis](https://docs.cavatica.org/docs/run-an-analysis-using-data-cruncher).
by clicking the **Data Studio** tab.
  - Click **Create new analysis**.
  - Select **RStudio**.
  - Use the default **Environment Setup**. You can read more about default and
  other available
  [environments and libraries for RStudio](https://docs.cavatica.org/docs/about-libraries-in-a-data-cruncher-analysis#rstudio).

## Project Setup

Before you begin, determine your working directory (`get(wd)` and `set(wd)`), and 
create two new folders within your preferred working directory entitled `data`
and `results`. You can copy and paste the following commands into the R console.

```r
dir.create("data")
dir.create("results")
```

## Data Sets

<!--
FIXME: place any data you want learners to use in `episodes/data` and then use
       a relative link ( [data zip file](data/lesson-data.zip) ) to provide a
       link to it, replacing the example.com link.
-->
Download the [data zip file](https://example.com/FIXME) and unzip it to your Desktop

## Software Setup

::::::::::::::::::::::::::::::::::::::: discussion

### Details

Setup for different systems can be presented in dropdown menus via a `spoiler`
tag. They will join to this discussion block, so you can give a general overview
of the software used in this lesson here and fill out the individual operating
systems (and potentially add more, e.g. online setup) in the solutions blocks.

:::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::: spoiler

### Windows

Use PuTTY

::::::::::::::::::::::::

:::::::::::::::: spoiler

### MacOS

Use Terminal.app

::::::::::::::::::::::::


:::::::::::::::: spoiler

### Linux

Use Terminal

::::::::::::::::::::::::

