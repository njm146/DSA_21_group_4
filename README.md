DSA_21_group_4
Project Name: Minimum Spanning Trees in Solving Optimal Network Setup
Group Mmbers: Nicholas Meegan (njm146, njm146@scarletmail.rutgers.edu), Christopher Rosenberger (cor9, cor9@scarletmail.rutgers.edu)

Project Idea: When attempting to connect a particular set of components - whether it be connecting cities with roads or a set of computers on a Wi-Fi network- 
the desire is to connect these components in an optimal way. By ensuring that the most efficient connections are made, it is possible to save time, money, or both depending on 
the application. Minimum spanning trees can be utilized to solve these types of problems. Given a graph that is undirected and all components in the graph are connected with edge 
weights, a minimum spanning tree can be formed. A minimum spanning tree contains no cycles and connects the edges in the graph such that the distance between all of the vertices 
is minimized. Therefore, each component in the minimum spanning tree is still connected to one another as in the initial graph, though the total distance to reach each component 
is the smallest out of all possible acyclic connections. Depending on the edge weights, there may be multiple minimum spanning trees possible. To determine the minimum spanning 
tree of a given graph of cities, computers, or any type of network, two algorithms will be analyzed in detail: Prim’s algorithm and Kruskal’s algorithm. Each algorithm will 
consist of three different implementations, varying the data structure used to form the minimum spanning tree, including a list implementation, binary heap implementation, and 
Fibonacci heap implementation from the Python fibheap library.

Code Instructions: To run the dataset generation code, use the following string of inputs: py datasetgen.py <Number of Vertices> <Dense/Sparse> <File to Save Dataset to>. 
This will generate a new dataset with the specified number of vertices and whether or not the graph is a dense graph or sparse graph.
Furthermore, tests for Prim’s or Kruskal’s algorithm can be run using prim.py and kruskal.py, respectively.  
To run these files, a string of inputs like the following need to be used: py <prim.py/kruskal.py> <graphFile>.  
Running either of these files will produce the weight of the MST calculated using a list, binary heap, and Fibonacci heap and print the results to the terminal.
Timing tests can be done using timing.py.  To run this file a string of inputs like the following is needed: 
py timing.py <numIterations> <outputFile> <graphFile1> <graphFile2> <graphFile3>... Note: Any number of graphs to test can be specified.  
After this, numIteration trials (needs to be an integer) will be performed on each graph specified using all three data structures specified on both Prim’s and Kruskal’s 
algorithm (6 functions in all).  The results of this, being the time taken, will be saved into the output file specified.

NOTE: It is necessary to install the "fibheap" library from Python to execute code. Ensure to run "pip install fibheap" in your command line terminal before running the
program.
