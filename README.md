
<!-- README.md is generated from README.Rmd. Please edit that file -->



`censys` is an R package interface to the [Censys API](https://censys.io/api)

Censys is a search engine that enables researchers to ask questions about the hosts and networks that compose the Internet. Censys collects data on hosts and websites through daily ZMap and ZGrab scans of the IPv4 address space, in turn maintaining a database of how hosts and websites are configured. Researchers can interact with this data through a search interface, report builder, and SQL engine.

[Censys tutorial](https://www.censys.io/tutorial).

The following functions are implemented:

- `censys_report`:	Create aggregate reports on the breakdown of a field in the result set of a query
- `censys_search`:	Perform queries against Censys data
- `get_series`:	Retrieve data on the types of scans Censys regularly performs ("series").
- `view_document`:	Retrieve data that Censys has about a specific host, website, or certificate.
- `view_result`:	Retrieve data on a particular scan "result"
- `view_series`:	Retrieve data that Censys has about a particular series

### News

- Version 0.1.0 released

### Installation


```r
devtools::install_github("hrbrmstr/censys")
```



### Usage


```r
library(censys)

# current verison
packageVersion("censys")
#> [1] '0.0.0.9000'
```

### Test Results


```r
library(censys)
library(testthat)

date()
#> [1] "Mon Jan 11 12:59:07 2016"

test_dir("tests/")
#> testthat results ========================================================================================================
#> OK: 0 SKIPPED: 0 FAILED: 0
```

### Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CONDUCT.md). 
By participating in this project you agree to abide by its terms.
