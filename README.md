# OS Principles

This repo contains various assignments I am working on for my Computer Operating Systems class

#### Matrix Multiplication - Multiprocessing
	$> gcc mm_proc.c
	$> ./a.out 1 2 3 4 1 2 3 4 1 3 2 4 1 3 2 4
	Child pid: 24129
	Child pid: 24130
	Parent pid: 24125
	Parent pid: 24125
	Exiting: 24129
	Child pid: 24128
	Parent pid: 24125
	Exiting: 24128
	Child pid: 24127
	Parent pid: 24125
	Exiting: 24127
	Child pid: 24126
	Parent pid: 24125
	The first row the resulting matrix is 16 36
	The second row of the resulting matrix is 16 36
	Display exiting
	Exiting: 24126
	Exiting: 24125

#### Matrix Multiplication - Multithreading
	$> gcc mm_threads.c -lpthread
	$> ./a.out 1 2 3 4 1 2 3 4 1 3 2 4 1 3 2 4
	Thread (0) being created
	Thread (1) being created
	Thread (2) being created
	Thread (3) being created
	Thread (4) being created
	Waiting for Display thread to finish if it hasnt already...
	Thread ID (1227265792)
	Waiting for matrix calculation threads to finish if they havent already...
	Thread ID (1235658496)
	C[3]=36
	Thread 3 exiting
	Thread ID (1244051200)
	C[2]=16
	Thread 2 exiting
	Thread ID (1252443904)
	C[1]=36
	Thread 1 exiting
	Thread ID (1260836608)
	C[0]=16
	Thread 0 exiting
	The first row the resulting matrix is 16 36
	The second row of the resulting matrix is 16 36
	Thread 4 exiting

#### Bounded-Buffer Producer/Consumer Problem - Multithreading
	$> gcc pc.c -lpthread
	$> ./a.out inputfile outputfile
