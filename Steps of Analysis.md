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

![11](https://user-images.githubusercontent.com/104814594/167105539-33d87e62-7abc-4564-acc5-388174a34155.JPG)

## 3. Data modelling
Using linear regression to find relationship within data.

```
summary(lm(carat~price, data=Dia))
par(mfrow=c(2,2))
plot(lm(carat~price, data=Dia))

```
# Output

```
Summary

Coefficients:
(Intercept)        price  
  0.3672972    0.0001095  
  
  ```
  
  ![12](https://user-images.githubusercontent.com/104814594/167106031-d70ec33e-a0e4-4597-8aff-9071bb40cd43.JPG)

