---
title: "Residual-Quantile Adjustment for Adaptive Training of Physics-informed Neural Network"
collection: talks
type: "Talk"
permalink: /talks/2022osaka
venue: "IEEE BigData 2022"
date: 2022-11-21
location: "Osaka, Japan"
---

Adaptive training methods for Physics-informed neural network (PINN) require dedicated constructions of the distribution of weights assigned at each training sample. To efficiently seek such an optimal weight distribution is not a simple task and most existing methods choose the adaptive weights based on approximating the full distribution or the maximum of residuals. In this paper, we show that the bottleneck in the adaptive choice of samples for training efficiency is the behavior of the tail distribution of the numerical residual. Thus, we propose the Residual-Quantile Adjustment (RQA) method for a better weight choice for each training sample. After initially setting the weights proportional to the p-th power of the residual, our RQA method reassigns all weights above q-quantile (90% for example) to the median value, so that the weight follows a quantile-adjusted distribution derived from the residuals. This iterative reweighting technique, on the other hand, is also very easy to implement. Experiment results show that the proposed method can outperform several adaptive methods on various partial differential equation (PDE) problems.
