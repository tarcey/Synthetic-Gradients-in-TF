# Synthetic Gradients in tensorflow 2.x

An example of synthetic gradients implemented as a tensorflow 2.x module.

The SGs are implemented as a tensorflow module. In the forwards-pass, the module simply passes through incoming values. In the backwards pass it intercepts incoming gradients and replaces them by synthetic gradients. The module is somewhat "plug-and-play", ie can be inserted in existing graphs with little additional effort. Details and limitations are commented in the code.
