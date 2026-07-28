---
title: Setup
---

For this lesson, you will be working in the R programming language and the 
RStudio development environment on the data analysis and sharing platform 
[CAVATICA](https://www.cavatica.org/).

## Setup

### Access CAVATICA

1. [Sign up for a free CAVATICA account](https://docs.cavatica.org/docs/sign-up-for-cavatica).

1. [Create a project](https://docs.cavatica.org/docs/quickstart#create-a-project). 
Give it a good descriptive name like `r-multiomics`.

1. For **Billing group**, select funds provided by the course or those that you 
have provided from your own funding source.

1. Under **Advanced settings**, change the default setting to 
`Allow network access`.
![Choose allow network access under advanced settings](./fig/allow-network-access.png)

1. Copy the `env-rstudio-multiomics` project into your new project.

1. Run a 
[Data Studio analysis](https://docs.cavatica.org/docs/run-an-analysis-using-data-cruncher) by clicking the **Data Studio** tab.

1. **Start** the `Motrpac-metaboAnalystR` analysis. This will take a few minutes to launch a machine instance. While it starts, notice that the **Environment** is RStudio.

  - Click **Create new analysis**.
  - Select **RStudio**.
  - Use the default **Environment Setup**. You can read more about default and
  other available
  [environments and libraries for RStudio](https://docs.cavatica.org/docs/about-libraries-in-a-data-cruncher-analysis#rstudio).

[contacting CAVATICA support](https://docs.cavatica.org/docs/getting-started).

### Use your own computer

R is a programming language that is especially powerful for data exploration, 
visualization, and statistical analysis. To interact with R, we use RStudio. 

1. Install the latest version of R from [CRAN](https://cran.r-project.org/).

2. Install the latest version of [RStudio](https://www.rstudio.com/products/rstudio/download/). 
Choose the free RStudio Desktop version for Windows, Mac, or Linux. 

3. Start RStudio. 

4. Install packages from R, Github, and Bioconductor. 

```r
install.packages(c("tidyverse", "ggrepel", "pak"))
library(pak)

# use `pak` to install the MoTrPAC analysis package and data
pak::pkg_install("MoTrPAC/MotrpacRatTraining6mo")

# install Bioconductor packages
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(c("pcaMethods", "edgeR", "MOFA2"))

```

Once the installation is complete, load the libraries to make sure that they 
installed correctly. 

```r
library(tidyverse)
library(ggrepel)
library(MotrpacRatTraining6mo)
library(pcaMethods)
library(edgeR)
library(MOFA2)

```

## Project Organization

1. Create a new project in your Desktop called `multiomics`. 
- Click the `File` menu button, then `New Project`.
- Click `New Directory`. 
- Click `New Project`.
- Type `multiomics` as the directory name. Browse to your Desktop to create the 
project there.
- Click the `Create Project` button.

2. Use the `Files` tab to create  a `data` folder to hold the data, a `scripts` 
folder to house your scripts, and a `results` folder to hold results. 
Alternatively, you can use the R console to run the following commands for step 
2 only. You still need to create a project with step 1.

```r
dir.create("./data")
dir.create("./scripts")
dir.create("./results")
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

