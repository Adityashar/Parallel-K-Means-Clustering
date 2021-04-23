# K-Means Clustering Algorithms

### For comparing and contrasting the performance of K-Means Clustering, three algorithms have been developed. 
The Sequential Algorithm is used as the base algorithm for the calculation of speedup with respect to the Amdahl's Law. OpenMP and Pthreads are used for parallelization of the algorithm.


- **Sequential**
  - `g++ main_sequential.c lab1_io.c Kmeans-Sequential.cpp -fopenmp -o seq.out`
  - `./seq.out 4 sample_dataset_50000_4.txt b.txt c.txt`
    
- **OpenMP**
  - `g++ main_omp.c lab1_io.c Kmeans-OpenMP.cpp -fopenmp -o omp.out`
  - `./omp.out 4 2 sample_dataset_50000_4.txt b.txt c.txt`
  
- **P-Threads**
  - `g++ lab1_io.c main_pthread.c Kmeans-Pthreads.cpp -o ptry.out -fopenmp`
  - `./ptry.out 4 2 sample_dataset_50000_4.txt b.txt c.txt`
  