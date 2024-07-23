---
contributor: max
date: '2023-10-24T08:08:10.490000+00:00'
title: 'A Performance-Portable SYCL Implementation of CRK-HACC for Exascale'
external_url: https://arxiv.org/pdf/2310.16122
authors:
  - name: Esteban M. Rangel
  - name: S. John Pennycook
  - name: Adrian Pope
  - name: Nicholas Frontiere
  - name: Zhiqiang Ma
  - name: Varsha Madananth
tags:
  - sycl
  - hpc
  - cuda
  - hip
  - heterogeneous-programming
---

The first generation of exascale systems will include a variety of machine architectures, featuring GPUs from multiple vendors.
As a result, many developers are interested in adopting portable pro- gramming models to avoid maintaining multiple versions of 
their code. It is necessary to document experiences with such program- ming models to assist developers in understanding the advantages and 
disadvantages of different approaches.
To this end, this paper evaluates the performance portability of a SYCL implementation of a large-scale cosmology application (CRK-HACC) 
running on GPUs from three different vendors: AMD, Intel, and NVIDIA. We detail the process of migrating the original code from CUDA to 
SYCL and show that specializing kernels for specific targets can greatly improve performance portability with- out significantly impacting 
programmer productivity. The SYCL version of CRK-HACC achieves a performance portability of 0.96 with a code divergence of almost 0, 
demonstrating that SYCL is a viable programming model for performance-portable applications.