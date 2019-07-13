# scm
software configuration management


## Open source stack

Install needs to work on CentOS 7 / RHEL 7

### Packages

Install the latest version of each of the following
- R 
- RStudio server CE
- Shiny server CE
- Anaconda for python 3

### R packages

Install the following R packages for all users (i.e. as root)
- those listed at https://github.com/Paradigm4/revealgenomics/blob/master/DESCRIPTION#L9
- `devtools`
- then the following special packages (commands taken from https://paradigm4.github.io/revealgenomics-docs/quickstart.html)
```sh
# in R 
# (potentially as root, so that all users have access to the package)
source('http://bioconductor.org/biocLite.R')
biocLite(c('Biobase'))

# in R 
# (potentially as root, so that all users have access to the package)
devtools::install_github('paradigm4/scidbr')
devtools::install_github('paradigm4/revealgenomics')
```
