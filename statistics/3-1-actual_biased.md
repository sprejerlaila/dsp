[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> 
```
import thinkstats2 as th
import thinkplot as thp
pmf = th.Pmf(resp.numkdhh, label='actual')

def biaspmf(pmf, label):
    new_pmf = pmf.Copy(label = label)
    for x, p in pmf.Items():
        new_pmf.Mult(x,x) #multiply the probability by x
    new_pmf.Normalize()
    return new_pmf

bpmf = biaspmf(pmf, label='observed') 

print('mean: ', pmf.Mean())
print('biased mean: ', bpmf.Mean())

thp.PrePlot(2)
thp.Pmfs([pmf, bpmf])
thp.Show(xlabel='number of children',ylabel='PMF')
```
>> mean:  1.024205155043831
>> biased mean:  2.403679100664282
