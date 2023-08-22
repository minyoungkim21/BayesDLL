# BayesDLL
### Bayesian Deep Learning Library

We release a new Bayesian neural network library for PyTorch for large-scale deep networks. Our library implements mainstream approximate Bayesian inference algorithms: **variational inference**, **MC-dropout**, **stochastic-gradient MCMC**, and **Laplace approximation**. The main differences from other existing Bayesian neural network libraries are as follows: 
**1)** Our library can deal with very large-scale deep networks including Vision Transformers (ViTs). 
**2)** We need virtually zero code modifications for users (e.g., the backbone network definition codes do not neet to be modified at all). 
**3)** Our library also allows the pre-trained model weights to serve as a prior mean, which is very useful for performing Bayesian inference with the large-scale foundation models like ViTs that are hard to optimise from the scratch with the downstream data alone. 

### *The technical report for the details of algorithms and implementation can be found in: [arXiv-URL-here].*

---

## Features

* Full implementation (without relying on other libraries) and easy-to-use demo codes for: **variational inference**, **MC-dropout**, **stochastic-gradient Langevin dynamics**, and **Laplace approximation**.
* Uncertainty quantification measures provided (eg, **ECE**, **MCE**, **Reliability plots**, **Negative log-likelihood scores**).
* Tested with ResNet-101 and ViT-L-32 -- Ready to be applicable to other Foundation models (eg, LLAMA, RoBERTa, Denoising Diffusion generative models) without code modification at all!
* Minimal (acceptable) use of extra computational resources (time & GPU memory) -- See our technical report.
* Detailed algorithmic details described/summarized in our technical report in arXiv.


## Environment setup
