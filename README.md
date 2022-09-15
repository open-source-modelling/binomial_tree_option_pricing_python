<h1 align="center" style="border-botom: none">
  <b>
    🐍 Binomial tree pricing model 🐍     
  </b>
</h1>


## Problem
A simple and fast model to price an European option with simple assumptions

## Solution
Binomial asst pricing model 
Inputs:
-  `N` ... # of time intervals
-  `T` ... time to maturity
-  `S_0` ... initial stock price
-  `sigma` ... volatility
-  `r` ... risk-free interest rate
-  `K` ... strike price
-  `isCall` ... is the option a call option (or a Put option if false)

## Getting started
Assuming that we are interested in an European call option that matures in 5 years. The pricing is done monthly so the number of time intervals is 5*12 months = 60.
The calculated volatility is 10 %, the risk-free rate is 5% and the strike price is 100. To get the implied price:
``` bash
import numpy as np
binom_tree_option(60, 5, 100, 0.1, 0.05, 100, False)
```
