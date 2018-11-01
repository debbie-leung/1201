# Continuous Distributions {#chap4}

Devore, Chapter 4

## Normal distribution

$P(Z \leq -1)$

Unless specified otherwise, `pnorm` uses a mean of 0 and standard deviation of 1 (standard normal).


```r
pnorm(-1)
```

```
## [1] 0.1586553
```

$P(X \leq 37)$ given $\mu = 40$ and $\sigma = 2$

```r
pnorm(37, mean = 40, sd = 2)
```

```
## [1] 0.0668072
```

or


```r
pnorm((37-40)/2)
```

```
## [1] 0.0668072
```

$P(X > 39)$

```r
1 - pnorm(39, mean = 40, sd = 2)
```

```
## [1] 0.6914625
```

Find the 75th percentile for the standard normal distribution:

```r
qnorm(.75)
```

```
## [1] 0.6744898
```

Find the 75th percentile for a normally distribution population with mean 40 and standard deviation 2:

```r
qnorm(.75, mean = 40, sd = 2)
```

```
## [1] 41.34898
```

or

```r
40 + qnorm(.75)*2
```

```
## [1] 41.34898
```
