# Python_for_Economists_Exam


### Python for the Financial Economist
Python for the Financial Economist is a masters course available on CBS for eligible students.
The course includes topics as quantitive finance including portfolio construction, fixed income, asset allocation, portfolio optimization, Black-Litterman views, advanced statistics and more.
This is all taught directly in Python notebooks, and all assignments including the exam is expected to be done using Python to implement course material.


### Exam
The exam is a two-parter, first part conserning Portfolio Diversification and the second part Portfolio Optimization. In this library a notebook is provided to each part. 

#### Part 1: Portfolio Diversification

As a measure of portfolio diversification Effective Number of Consituents (ENC) are used, as it highlights concentration in the portfolio (or inversely; diversification). However fails to include correlation structure among the assets included, thus the portfolio risk (volatility) is deconstructed using Euler principle and findings of said deconstruction are discussed.

Another diversification measure is introduced, essentially estimating the risk per asset as a stand-alone risk weight out of the entire portfolio risk - the latter including covariance structure. 
Upon having calculated said risk measure solve an optimization problem, with the target being maximized risk by maximizing the aforementioned measure subject to a long-only, no leverage constraint.

This is compared to the minimum-variance portfolio, also solved for.

Finally, we evaluate the optimized portfolios with calculation of information ratio and Turn-over against common academically used benchmarks such as the market portfolio or the equal-weighted portfolio.

As data the Fama-French 49 industry portfolios are retrieved using the API connecting to Kenneth Frenchs website data library.


#### Part 2: Portfolio Optimzation

Given initial wealth, covariance structure and expected returns the aim is to maximize wealth over a period of time. 
Initially the distribution and statistically relevant properties of the asset holdings are described.

Given a buy and hold strategy is desired and the investor faces described transaction costs, we aim to optimize the portfolio with the target function being a power utility function, with a 5Y time horizon, which can be re-written into a satisfaction measure. We optimize over the satisfaction measure, subject to long only (buy-and-hold) constraints and acccounting for transaction costs. 

Finally, we evaluate the optimized strategy through visual representation of allocation alongside risk calculations including volatility and conditional VaR. 

