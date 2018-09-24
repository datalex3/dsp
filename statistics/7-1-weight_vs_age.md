[Think Stats Chapter 7 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2008.html#toc70) (weight vs. age)

import first

def SpearmanCorr(xs, ys):

    xranks = pd.Series(xs).rank()
    
    yranks = pd.Series(ys).rank()
    
    return Corr(xranks, yranks)
    
def Corr(xs, ys):

    xs = np.asarray(xs)
    
    ys = np.asarray(ys)
    
    meanx, varx = thinkstats2.MeanVar(xs)
    
    meany, vary = thinkstats2.MeanVar(ys)

    corr = Cov(xs, ys, meanx, meany) / np.sqrt(varx * vary)
    return corr
    
live, firsts, others = first.MakeFrames()

live = live.dropna(subset=['agepreg', 'totalwgt_lb'])

ages = live.agepreg

weights = live.totalwgt_lb

print('Corr', Corr(ages, weights))

print('SpearmanCorr', SpearmanCorr(ages, weights))

Corr 0.0688339703541

SpearmanCorr 0.0946100410966


