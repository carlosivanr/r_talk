# Introduction to R Workshop
- California State University, Chico
- Department of Psychology
- Author: [Carlos Rodriguez](https://keen-wilson-61a022.netlify.app/), PhD. Mind Research Network
- Date: February 16, 2022

<!-- [**Download the workshop materials by clicking here**](https://github.com/carlosivanr/intro_to_R/). -->

## Pre-workshop instructions
In this workshop, we will be covering basic commands in R to get users over the hump of learning R.

**Install Software** \
A working installation of both R and RStudio is required. R and RStudio are two completely different things. R is the core programming language and RStudio is an integrated development environment (IDE) that makes working with R easier.
- [Install R](http://cran.wustl.edu/)
- [Install RStudio](https://www.rstudio.com/products/rstudio/download/#download)

**Install Packages** \
When installing R, you are getting a base version with a set of built-in functions. We can add features and functionality to R by installing and then loading packages. These packages will have additional functions and some will have built-in data sets to practice executing functions.

- Open RStudio
- Click on the "Console" tab in the left hand pane of RStudio
- To install packages, use the `install.packages()` function. This function takes the name of the package to be installed encased in single or double quotes as its input argument. The following commands can be copy-pasted and then run in the RStudio Console.
 ```{r}
 install.packages("tidyverse")
 install.packages("rstatix")
 install.packages("ggpubr")
 install.packages("AMCP")
 ```

**Load Packages** \
Once a package is installed, it needs to be loaded into the R Session to become available for use. Packages need to be loaded during each session. To load a package, use the `library()` function. Simply pass in the name of the package, with out quotes as its input. The following can be copy pasted into the console.
 ```{r}
 library(tidyverse)
 library(rstatix)
 library(ggpubr)
 library(AMCP)
 ```
 
 **Function Name Conflicts** \
 Every now and then you may load a package that contains functions with overlapping names. Usually these come up in a warning messages when loading a package. To avoid confusion, you can specify the package and function in code. This is usually written as the package name, double colons, and then the function. This is helpful for troubleshooting errors in code.
 ```{r}
 # Normal call to the select function
 select(data_frame, column_to_select)
 
 # Specifying the select function from the dplyr package
 dplyr::select(data_frame, column_to_select)
 ```
 

