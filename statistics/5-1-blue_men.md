[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> 
```
import brfss
import scipy
import scipy
def BlueMan(maxh, minh):    
    males = df[df.sex == 1]
    mean = males.htm3.mean()
    std = males.htm3.std()
    high = scipy.stats.norm.cdf(maxh, loc=mean, scale = std)
    low = scipy.stats.norm.cdf(minh, loc=mean, scale = std)
    dif = high - low
    return di

BlueMan(185.42,177.8)
```
>> 0.3432308764365409
