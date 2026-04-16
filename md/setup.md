---
title: "Data & setup"
number-sections: false
---

<!-- 
Note for Training Developers:
We provide instructions for commonly-used software as commented sections below.
Uncomment the sections relevant for your materials, and add additional instructions where needed (e.g. specific packages used).
Note that we use tabsets to provide instructions for all three major operating systems.
-->

## Data

The data used in these materials is provided as a zip file. 
Download and unzip the folder to your Desktop to follow along with the materials.

<!-- Note for Training Developers: add the link to 'href' -->
<a href="">
  <button class="btn"><i class="fa fa-download"></i> Download</button>
</a>

## R/Python installation

::: {.panel-tabset group="language"}
## R

#### Required software

- [Download R](https://cran.r-project.org/) and install it using default options. (Note: choose the "base" version for Windows)
- [Download RStudio](https://www.rstudio.com/products/rstudio/download/#download) and install it using default options. 

#### Setting up RStudio

After installing RStudio, change some of its default options (you only need to 
do this once): 

- From the upper menu go to <kbd>Tools</kbd> > <kbd>Global Options...</kbd> 
- _Untick_ the option "Restore .RData to workspace on startup."
- Change "Save workspace to .RData on exit" option to "Never"
- Press <kbd>OK</kbd>

## Python

For this course we recommend using [Visual Studio Code](https://code.visualstudio.com). This provides support for various programming languages (including Python and R). It works on Windows, MacOS and Linux. It's also open-source and free.

Please refer to the [installation instructions](https://code.visualstudio.com/docs/python/python-tutorial) and make sure that you verify that Python code will run.

A brief sequence of events:

1. Install Visual Studio Code
2. Install the VS Code Python extension
3. Install a Python interpreter
    * Windows: install from [Python.org](https://www.python.org/downloads/) or use the Microsoft Store
    * MacOS: install the [Homebrew](https://brew.sh) package manager, then use this to install Python
    * Linux: comes with Python 3, but needs `pip` to install additional packages
:::


## Packages
We will be using the following packages throughout this course:

::: {.panel-tabset group="language"}
## R

You'll need the following packages:

```{r}
#| eval: false
install.packages("tidyverse",
                 "survival",
                 "survminer")
```


## Python

-   `numpy`
-   `pandas`
-   `lifelines`
-   `matplotlib`

These can be be installed either via `pip`, for example:

```{python}
#| eval: false
pip install numpy
```
or via `conda`:

```{python}
#| eval: false
conda install -c conda-forge numpy
```
:::