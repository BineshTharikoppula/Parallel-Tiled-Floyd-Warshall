# Parallel-Tiled-Floyd-Warshall
Parallel Implementation and Analysis of All Pairs Shortest Path Algorithm(Floyd-Warshall Algorithm) using OPENMP C++ library and Comparing Runtimes of Parallel Tiled FW Algorithm with Parallel Standard FW Algorithm.

Hai Guys..
   
   FinalAPSP.cpp --> is source code file which is having implementation of both Parallellized Tiled FW algorithm and Parallellized     standard FW algorithms.And runtimes of both will be displayed as output even if you want to print All pairs shortest path matrix you can print that on console.
   
sample.txt,sample2.txt,sample3.txt --> is input file for above program which contains graph.

For Example:
   Input Graph i.e.. Adjacency Matrix Will be Given As
   Ex:
 	[0    3         Infnity  7       ]
 	[8    0         2        Infinity]
 	[5    Infinity  0        1       ]
 	[2    Infinity  Infinity 0       ]

  This Matrix Will be Given Input from txt file As
  Like This..

  c no-of-vertices no-of-edges 
	p sp 4 7
	c from to edge-weight 
	a 1 2 3
	a 2 1 8
	a 2 3 2
	a 3 1 5
	a 3 4 1
	a 4 1 2
	a 1 4 7 

 Explanation:
   
  -> Line Starts With 'c' is considered as comments in program means it will be omitted.

  -> Line Starts With 'p' contains 3 arguments more
  		1. sp--Graph Type
  		2.Number of Vertices.
  		3.Number of Edges

  -->Line Starts With 'a' contains 3 arguments more
        1.Node From where Edge Starts.
        2.Node To Where Edge Connected.
        3.Weight of the Edge.

  After filling these values from txt to Adjacency Matrix, 
  Fill the Remaining Values With Infinity(Programmatically INT_MAX)
  Except Diagonal Values which are Logically Zero.
  
  
  
