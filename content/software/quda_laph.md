---
title: quda_laph
external_url: https://github.com/cosmon-collaboration/quda_laph
software_type: hpc
repo: github
summary: quda_laph performs lattice QCD computations with stochastic Laph and distillation using the QUDA library.
---

Quda_laph carries out lattice QCD computations involving Laplacian-Heaviside (LapH) smeared Wilson-type quarks. It utilizes the QUDA library in order to carry out its calculations on GPUs. It uses no other libraries, except HDF5 (in the future) and those needed by QUDA. An installed library of QUDA is needed, compiled using the CUDA or ROCm toolkit. The installed QUDA library does NOT need to be compiled with any of the USQCD helper libraries, such as QIO, QMP, QDP, or Chroma. QUDA must be compiled with QUDA_INTERFACE_QDP=ON since QDP ordering of the lattice sites is used on the hosts, but all other USQCD interfaces can be safely turned OFF. Either a serial or an MPI-based parallel implementation with or without OpenMP threads can be compiled.
