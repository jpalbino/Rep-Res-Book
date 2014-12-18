# [Reproducible Research with R and RStudio (Second Edition)](http://christophergandrud.github.io/RepResR-RStudio/)

[<img src="http://3.bp.blogspot.com/-f8MFbNEoyGU/UYNGekqEkTI/AAAAAAAAGOM/Dq36pI06kTQ/s320/RepResCover.jpg" align="right" />](http://www.amazon.com/dp/1466572841)

[Christopher Gandrud](http://christophergandrud.blogspot.com/p/biocontact.html)

[CRC Press/Chapman & Hall](http://www.crcpress.com/product/isbn/9781466572843)

The files in this repository comprise the source code for creating
**Reproducible Research with R and RStudio**.

### File Organization

The main files used to create the manuscript of the book are in the `Source`
folder. This folder contains the parent *knitr* `.Rnw` file in the
`Source/Parent/` directory. Child documents for the book chapters are in the
`Source/Children/` directory and child files for the book's front matter are in
the `Source/FrontMatter/` directory.

### Reproduce the Book

The book can be reproduced by using the R package *knitr*. To do this:

1. Make sure you have [R](http://www.r-project.org/), [LaTeX](http://www.latex-project.org/ftp.html),
and the *knitr* R package installed on your computer. Also install Andre Simon's
[highlighter utility](http://www.andre-simon.de/zip/download.html).

2. Download this repository and point the directories in the *BookMake.R* make
file to where it is downloaded to.

3. Run the *BookMake.R* make file in R.

Note: To install the R packages used to compile the book open the
*Source/Children/FrontMatter/Packages.Rnw*. Find:

```
doInstall <- FALSE
```

in the code chunk labeled "FrontPackageCitations". Change the value `FALSE` to
`TRUE` and run the code chunk.

**Note:** the LaTeX file will compile with errors and warnings. These are
related to stylistic choices and should largely be ignored. But because of this
you will need to **compile the document a few times** to get the full text with
bibliography and index.

#### Reproducing the Book in Windows.

If you would like to reproduce the book and are using Windows you will need to
install [RTools](http://cran.r-project.org/bin/windows/Rtools/installer.html).
Please use the recommended installation to ensure that your system PATH is set
up correctly. Otherwise your computer will not know where the tools are.

#### Reproducing this Book in Linux

You will need to install the the R packages RCurl and XML seperately. See
[this post](https://github.com/cboettig/treeBASE/issues/5) for more details.

### Session Info

The current version of the book manuscript was compiled with
[RStudio](http://www.rstudio.com/) (v. 0.98.880 developer build) with the
following R session:


```
## R version 3.1.2 (2014-10-31)
## Platform: x86_64-apple-darwin14.0.0 (64-bit)
## 
## locale:
## [1] en_GB.UTF-8/en_GB.UTF-8/en_GB.UTF-8/C/en_GB.UTF-8/en_GB.UTF-8
## 
## attached base packages:
## [1] splines   stats     graphics  grDevices utils     datasets  methods  
## [8] base     
## 
## other attached packages:
##  [1] ZeligBayesian_0.1   MCMCpack_1.3-3      coda_0.16-1        
##  [4] lattice_0.20-29     Zelig_4.2-1         sandwich_2.3-2     
##  [7] MASS_7.3-35         boot_1.3-13         xtable_1.7-4       
## [10] WDI_2.4             ROAuth_0.9.5        texreg_1.34        
## [13] survival_2.37-7     stargazer_5.1       rvest_0.1.0.9000   
## [16] RJSONIO_1.3-0       rmarkdown_0.4.1     reshape2_1.4.1     
## [19] repmis_0.3.3        RCurl_1.95-4.5      bitops_1.0-6       
## [22] quantmod_0.4-3      TTR_0.22-0          xts_0.9-7          
## [25] zoo_1.7-11          markdown_0.7.4      magrittr_1.5       
## [28] knitr_1.8.4         knitcitations_1.0.5 httr_0.6.0         
## [31] googleVis_0.5.6     ggplot2_1.0.0       formatR_1.0        
## [34] extrafont_0.17      dplyr_0.3.0.2       digest_0.6.6       
## [37] devtools_1.6.1      data.table_1.9.4    countrycode_0.17   
## [40] brew_1.0-6          animation_2.3      
## 
## loaded via a namespace (and not attached):
##  [1] assertthat_0.1    bibtex_0.3-6      chron_2.3-45     
##  [4] colorspace_1.2-4  DBI_0.3.1         evaluate_0.5.5   
##  [7] extrafontdb_1.0   grid_3.1.2        gtable_0.1.2     
## [10] highr_0.4         htmltools_0.2.7   lubridate_1.3.3  
## [13] memoise_0.2.1     munsell_0.4.2     parallel_3.1.2   
## [16] plyr_1.8.1        proto_0.3-10      R.cache_0.10.0   
## [19] R.methodsS3_1.6.1 R.oo_1.18.0       R.utils_1.34.0   
## [22] Rcpp_0.11.3       RefManageR_0.8.40 rJava_0.9-6      
## [25] rjson_0.2.15      Rttf2pt1_1.3.2    scales_0.2.4     
## [28] stringr_0.6.2     tools_3.1.2       twitteR_1.1.7    
## [31] xlsx_0.5.7        xlsxjars_0.6.1    XML_3.98-1.1
```

---

(c) Christopher Gandrud (2014)
