# Calculate co-effecienct of Variance

### Instructions

1. Install:

         pip install conPov


2. Self convolution of discrete distribution

      #### import libraries
         from conPOV import main
         import numpy as np # for creating random series
         from scipy.stats import binom # for creating probability mass function
      #### example of probability mass function
         n = 10 # number of visitors selected randomly
         p = 0.80 # the probability that a visitor will end up buying a souvenir
         k = np.arange(0,11) # different possible number of visitors selected in a numpy array i.e. 0 or 5 etc
         # generate the probability distribution
         pmf_series = binom.pmf(k=k, n=n, p=p)
         n_fold = 2
      #### self convolution of discrete distribution
         # n-fold self convolution of discrete distribution
         result = main.ConPov(pmf_series, n_fold).conpov()
