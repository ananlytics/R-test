# Three basic degrees of analysis

## 1. Descriptive Analysis of Data.
Using Diamonds dataset to find mean and median using a single line code.
```
diamonds %>% summarise(mean_depth=mean(depth),median_depth=median(depth))

```
# Output

```
_# A tibble: 1 x 2
  mean_depth median_depth
       <dbl>        <dbl>
1       61.7         61.8_

```
