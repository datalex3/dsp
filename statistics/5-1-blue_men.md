[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

import scipy.stats

dist.mean(), dist.std()
(178.0, 7.7000000000000002)
dist.cdf(mu-sigma)
0.15865525393145741
low = dist.cdf(177.8)   
high = dist.cdf(185.4)  
low, high, high-low
(0.48963902786483265, 0.83173371081078573, 0.34209468294595308)

