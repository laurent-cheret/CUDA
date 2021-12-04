# CUDA Matrix Multiplication

The majority of CUDA examples available are for matrix multiplication using square matrices. This code calculates K multiplications (A1*B1 = C1; A2*B2 = C2; ...etc)of randomly generated matrices by using 3 dimensions for the threads and blocks on the GPU (threadIdx.x, threadIxd.y, threadIdx.z), and (blockDim.x, blockDim.y, blockDim.z). The "z" dimension is used as an indexer for each of the K matrices A and B.

In the first attempt the code iterates over each one of the A and B matrices to generate matrix C one at a time. The second attempt does the same by using the Z dimension in CUDA threads and blocks to index multiple matrices A and B at the same time and perform parallel multiplication.

