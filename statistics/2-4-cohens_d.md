[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

wgt_diff = firsts.totalwgt_lb.mean() - others.totalwgt_lb.mean()

var_firsts = firsts.totalwgt_lb.var()
var_others = others.totalwgt_lb.var()
n1, n2 = len(firsts.totalwgt_lb), len(others.totalwgt_lb)

pooled_var = (n1 * var_firsts + n2 * var_others) / (n1 + n2)
cohens_d = wgt_diff / np.sqrt(pooled_var)
cohens_d

-0.088672927072602006
