
# systemr

The goal of systemr is to run system command outside rstudio. Sometimes
Rstudio-Terminal does not behave exactly as normal terminals. For those
case, systemr can be used from a normal terminal to create a local api,
that will run system command.

## Installation

You can install the latest development version from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("benjaminguinaudeau/systemr")
```

## Example

Open a terminal and run. This will serve the api on the given port.

``` r
serve_cli(host = "localhost", port = 5000)
```

From your rstudio session, you can now run system\_api, whic will
execute the code in the terminal and transfer the output to rstudio.

``` r
system_api("pwd")
```
