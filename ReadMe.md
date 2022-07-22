# Calculate co-effecienct of Variance

### Instructions

1. Install:

        pip install conPov


2. Self convolution of discrete distribution

        from conPov import main
        # n-fold self convolution of discrete distribution
        result = main.ConPov(pmf_series, n_fold).conpov()
