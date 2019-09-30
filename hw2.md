p8105\_hw2\_yc3729
================
Yineng Chen
2019/9/29

``` r
mrtw_data = read_excel("./data/HealthyHarborWaterWheelTotals2018-7-28.xlsx",
                  sheet = 1,
                  range = "A2:N338") %>% 
  janitor::clean_names() %>% 
  drop_na(dumpster)
```

    ## Warning in FUN(X[[i]], ...): strings not representable in native encoding
    ## will be translated to UTF-8
