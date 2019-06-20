[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```python
resp = nsfg.ReadFemResp()

pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')
biased_pmf = BiasPmf(pmf, label='biased')

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Show(xlabel='number of children', ylabel='PMF')

actual_mean = pmf.Mean()
biased_mean = biased_pmf.Mean()

print('Actual Mean', actual_mean)
print('Biased Mean', biased_mean)
```

Returns:
Actual Mean 1.024205155043831
Biased Mean 2.403679100664282
