---
title: mpi_jm
external_url: https://github.com/cosmon-collaboration/mpi_jm
software_type: hpc
repo: github
summary: Mpi_Jm (MPI Job Manager) is a system for efficiently bundling related tasks for supercomputing.
---

mpi_jm Objectives:

- Efficiently run a large set of jobs of bounded size in a large allocation of nodes.
- Solve node fragmentation function. Repeated launch and completion of jobs leaves available nodes spread out with poor interconnect performance.
- Automate binding of node resources, picking the right cores to match GPU use, setting affinity for openMP threads.
- Support overlay of jobs using distinct resources on the same nodes, i.e. GPU vs CPU jobs.
- Jobs support pre and post actions that can be used to chain computations with simple dependencies.
- Customizable collection of workload with python based frontend.
- Dynamic dependencies - jobs can wait for set of prerequisite conditions like completion of a job with neighboring parameters.
- Python based runtime estimation. Can implement machine learning model configured on prior run data.
- Dynamic reconfiguration of jobs to compute inside allocation time.
