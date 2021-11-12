# Convolutional Neural Networks

## Points
- Efficient models for natural signals.

- c.p **Fully-connected** layers applied on **tabular data**: no prior assumption on how features interact.

----
## Natural Signal Properties


### Locality ↔ Sparsity / Receptive Field
Nearby pixels/points are more correlated with each other than pixels/points far away. <br>
e.g. X[0,0] is blue → high probability that the next pixel is also blue. 

Connection sparsity : Drop connections between far away neurons. 

### Stationarity / Spatial Invariance ↔ Parameters (weights) sharing
Similar patterns repeat throughout a signal / in different regions of an image.

Convolution kernel: use a small set of parameters multiple times across the network structure. 

### Compositionality ↔ Stacking of layers
Everything in nature is composed of parts that are composed of sub-parts. 

----
## References
[Properties of natural signals -- Alfredo Canziani](https://atcold.github.io/pytorch-Deep-Learning/en/week03/03-3/)
