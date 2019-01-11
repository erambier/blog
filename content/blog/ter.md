---
title: "Master 1 Thesis, European Option Pricing"
date: 2016-05-19
draft: false
---
&nbsp; My master 1 endend with a [thesis](/files/ter.pdf). Along with my team mate Inés, we choosed to dig into European Option Pricing. The problem was challenging since both of us didn't have any kind of background in finance.    
 In a nut shell, an european option is a contract which gives the buyer (the owner or holder of the option) the right, but not the obligation, to buy or sell an underlying asset or instrument at a specified strike price on a specified date. The goal of this project was to clearly differentiate the pricing of the option and the portofolio management to cover a put lower that a call. We organized our approach with two parts:

&nbsp; &nbsp; The first part deals with the modeling of the problem. Before tackling the famous Black-Scholes formula, we first dissected a model based on the discret version of the stock market. The Cox-Ross-Rubinstein binomial option pricing model (CRR model) traces the evolution of the option's key underlying variables in discrete-time. This is done by means of a binomial lattice (tree), for a number of time steps between the valuation and expiration dates. Each node represents a possible price at a given point in time. Valuation is performed iteratively, starting at each of the final nodes (those that may be reached at the time of expiration), and then working backwards through the tree towards the first node (valuation date). The value computed at each stage is the value of the option at that point in time. 
Then we prooved than the binomial model value converges on the Black–Scholes formula value as the number of time steps increases. Also we verified that the binomial distribution of the price approaches the lognormal distribution assumed by Black–Scholes.
From this, we implemented in MatLab the analytical solution of pricing, and simulate a portofolio managemnent from real life data found on Yahoo finance.  

&nbsp; &nbsp; The second part of the project aims to answer the estimation of the standard deviation. The so-called future volatility is the only parameter of the Black-Scholes formula that couldn't be calculate from the past values. The volatility is a famous for its complexe estimatimation and its capabilities to completely jeoperdize the robustness of the Black-Scholes formula. We tried to draw rigorous conclusions on the volatility fluctiation and explored the different solutions to estimate it.


Find the rapport [here](/files/ter.pdf).
