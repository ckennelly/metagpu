metagpu - JIT-based Template Metaprogramming for GPU Development
(c) 2013 - Chris Kennelly (chris@ckennelly.com)

Overview
========

metagpu is a header-based library for constructing GPU-based kernels entirely with a standard C++ compiler.  Rather than rely on a specialized compiler for GPU-based code at compile time, device code is generated at runtime on-the-fly.  Besides eliminating an additional compiler dependency, this approach allows for runtime code to be more finely retargeted according to the hardware available.  In the future, a tradeoff could be made between vectorized x86 host code and GPU-based device code without programmer intervention.

Limitations
===========

* metagpu currently only targets CUDA-based architectures.
