# Synthetic Gradients in TF 2.x

I couldn't find any example implementation of synthetic gradients for tensorflow 2.x, so here is one. The SGs are implemented as a tensorflow module. In the forwards-pass, the module just passes through incoming values. In the backwards pass it intercepts incoming gradients and replaces them by synthetic gradients. The module is somewhat "plug-and-play", ie can be inserted in existing graphs with little additional effort. Details and limitations are commented in the code.

This is a snapshot of a messy colab notebook that i only use for educational experiments like this, but i did put in some effort to clean up the parts relevant to synthetic gradients, enough to serve as an educational example.
