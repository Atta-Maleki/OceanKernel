# OceanKernel
The Ocean Kernel algorithm is a benchmarking algorithm that measures the performance of processors. It can be run on multiple types of processors, including CPUs and GPUs, and can be executed using different strategies. The algorithm can be run sequentially or in parallel. However, the sequential version of the algorithm is not as fast as the parallel version. The main goal of the algorithm is to measure how different parallel strategies work and what results they produce.

Parallel on GPU
---
When running the algorithm in parallel on a GPU, we use CUDA, which is the fastest way possible. The GPU handles all the calculations by splitting and assigning each calculation to a thread on many cores. Because of the existence of many cores inside the GPU, the calculations are completed quickly.

Parallel on CPU
---
When running the algorithm in parallel on a CPU, we can assign some tasks to each core and see how they work. There are two methods to do this. The first method is similar to CUDA but on a smaller scale using OpenMP. The second method is Message Passing( MPI ), which is completely different. In the Message Passing method, some tasks are assigned to each core. They have their own data, do the calculations, and if there is any resource that should be shared, they ask for the data from other owners. The difference between the two methods is the resource sharing method.
