# web-scraping-with-R
Examples for web-scraping and text analysis with R

## Installation
### Installing all required packages
Run the following lines first in R console to install required packages:
```r
for (pkg in c("rvest","httr","dplyr","stringr","XML","RCurl","ggplot2","reshape","tm","ggmap")){
 if (!pkg %in% rownames(installed.packages())){install.packages(pkg)}
}
```

### Checking out this repository
Then, in RStudio,

1. Select `File -> New Project... -> Version Control -> Git` 
2. Paste `https://github.com/ubcecon/web-scraping-with-R` (the URL for this repo) into the space for `Repository URL`. Press on `Create Project`.

or simply clone this repo using your favourite Git client to checkout this repository.

Once the repo is checked out, try replicating the following examples by yourself by opening the corresponding `.Rmd` files:

## Tutorials
### [EPS trend difference by industry from Yahoo Finance](yahoo-finance.md) (`yahoo-finance.rmd`) by @jasminehao
Basic principles of web scraping by URL patterns and HTML parsers.
### [Real-time data mining from Yahoo Finance](yahoo-realtime.md) (`yahoo-realtime.rmd`) by @jasminehao
Web scraping for data that are chaging real-time.
### [Economic literature analysis from AER abstracts](aer-articles.md) (`aer-articles.rmd`) by @chiyahn
HTML/CSS analysis using `SelectorGadget` and developer tools for `rvest` & principles of basic text analysis with beautiful wordclouds.
### [Cross-industry firm location differences from SEC website](sec-location.md) (`sec-location.rmd`) by @chiyahn and @jasminehao
Web scraping from query-based webpages and geocoding.

## Resources
Relevant R packages and developer tools:
- `rvest` (HTML parsing): https://github.com/hadley/rvest
- `tm` (text mining and analysis): http://tm.r-forge.r-project.org/
- `SelectorGadget` (HTML/CSS analysis): https://selectorgadget.com/

Useful R packages for data cleaning:
- PSID: https://github.com/floswald/psidR
- The World Wealth and Income Database: https://github.com/WIDworld/wid-r-tool
- The Survey of Professional Forecasters: https://github.com/joergrieger/Survey
