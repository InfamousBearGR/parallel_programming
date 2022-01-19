# parallel_programming
Rosenbrock function done prallel in C.

A University project. Given the Rosenbrock function in C we were tasked to make it work in parallel using:
1. OpenMP
2. OpenMP Tasks
3. MPI
4. MPI and OpenMP

The report is in Greek. To run the files use the following commands:

- For OpenMP:  
  `gcc -fopenmp -O3 -o multistart_hooke_omp multistart_hooke_omp.c`  
  `./multistart_hooke_omp`

- For OpenMP Tasks:  
  `gcc -fopenmp -O3 -o multistart_hooke_omp_tasks multistart_hooke_omp_tasks.c`  
	`./multistart_hooke_omp_tasks`

- For MPI:  
  `mpicc -g -O3 -o multistart_hooke_mpi multistart_hooke_mpi.c`  
	`mpirun -c 6 multistart_hooke_mpi`
  
- For MPI and OpenMP:  
  `mpicc -g -O3 -fopenmp -o multistart_hooke_mpi_omp multistart_hooke_mpi_omp.c`  
	` mpirun -c 6 multistart_hooke_mpi_omp`
