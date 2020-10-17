# programming-techiniques-for-supercomputers

1.Download the program

2.Using terminal check whether Gcc is installed or not! ( gcc --version )

3.Igonre this if it shows some version. If not run this command in termianl ( sudo apt install gcc )

4.Configuring OpenMP-We can check whether the OpenMP features are configured into our compiler or not, using the command ( echo |cpp -fopenmp -dM |grep -i open )
   If OpenMP is not featured in the compiler, we can configure it use using the command ( sudo apt install libomp-dev )
   
5.Setting the number of threads-In OpenMP, Before running the code, we can initialise the number of threads to be executed using the following command. Here, we set the number of   threads to be getting executed to be 8 threads. ( export OMP_NUM_THREADS=8 )

6.Compile: ( gcc -o cmp -fopenmp your_c_program_name.c )

7.Execute: ( ./cmp )
