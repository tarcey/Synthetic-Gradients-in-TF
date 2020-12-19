# Synthetic Gradients in tensorflow 2.x


An implementation of synthetic gradients (described in Deepmind's 2017 paper) as a reusable tensorflow 2.x module.


In the forwards-pass, the module simply passes through incoming values. In the backwards pass it intercepts incoming gradients and replaces them by synthetic gradients. The module is somewhat "plug-and-play", ie can be inserted in existing graphs with little additional effort. Details and limitations are commented in the code.

The synthetic gradients are tested on a text-classification task using attention & positional encoding on the sentiment140 dataset.
