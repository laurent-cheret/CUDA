# CUDA

The majority of CUDA examples available are for matrix multiplication using square matrices. This code calculates K multiplications (A1*B1 = C1; A2*B2 = C2; ...etc)of randomly generated matrices by using 3 dimensions for the threads and blocks on the GPU (threadIdx.x, threadIxd.y, threadIdx.z), and (blockDim.x, blockDim.y, blockDim.z). The "z" dimension is used as an indexer for each of the K matrices A and B.
