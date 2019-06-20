[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```python
random_1000 = np.random.random(1000)

random_pmf = thinkstats2.Pmf(random_1000)

thinkplot.Pmf(random_pmf)
thinkplot.Config(ylabel='probability', xlabel='value')
```

There are lines at every intermediate value, making meaningful observations impossible.

```python
random_cdf = thinkstats2.Cdf(random_1000)

thinkplot.Cdf(random_cdf)
thinkplot.Config(ylabel='CDF', xlabel='value')
```
