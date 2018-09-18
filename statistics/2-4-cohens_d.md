[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> 
'''
import math\
def CohenEffectSize(grup1, group2):\
  diff = group1.mean() - group2.mean()\
  var1 = group1.var()\
  var2 = group2.var()\
  n1,n2 = len(group1), len(group2)\
  pooled_var = (n1*var1 = n2*var2) / (n1+n2)\
  d = diff / math.sqrt(pooled_var)\
  return d

first_wgt = first.totalwgt_lb\
first_lgt = first.prglngth

rest = preg[preg.pregordr!=1]\
rest_wgt = rest.totalwgt_lb\
rest_lgt = rest.prglngth

print('Difference in weight: ', CohenEffectSize(first_wgt, rest_wgt))\
print('Difference in length: ', CohenEffectSize(first_lgt, rest_lgt))
'''
>> Difference in weight:  -0.06911825348820934\
>> Difference in length:  -0.03131178583370273
