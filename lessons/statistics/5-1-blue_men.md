[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```python
import scipy.stats

mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)

def imperial_to_cm(feet, inches):
    return 2.54 * (12 * feet + inches)

print(100 * (dist.cdf(imperial_to_cm(6, 1)) - dist.cdf(imperial_to_cm(5, 10))),
     '% of males are in the 5\'10" to 6\'1" height range')
```

Returns:
34.27468376314746 % of males are in the 5'10" to 6'1" height range
