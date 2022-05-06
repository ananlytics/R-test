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

## 2. Visual Analysis of Data.
Using Diamonds dataset to plot columns using a single line code.
```
ggplot(aes(x=carat,y=price),data=subset(Dia,clarity=="VVS1"))+geom_point(color="Green")+scale_x_discrete(breaks=seq(0,3,0.5))
lm(carat~price, data=Dia)

```
# Output

```
![11](https://user-images.githubusercontent.com/104814594/167105394-a1477f0d-bf58-46c2-870c-bce842222f1f.JPG)

```

