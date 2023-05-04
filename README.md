Download Link: https://assignmentchef.com/product/solved-csci203-csci803-assignment-3-shortest-path
<br>
This assignment involves an extension to the single source – single destination shortest path problem.




<h1>The Program</h1>




Your program should:

<ol>

 <li>Open the text file “ass3.txt”. (Note: “ass3.txt” should be a hardcoded as a constant.)</li>

 <li>Read a graph from the file.</li>

 <li>Find the shortest path between the start and goal vertices specified in the file.</li>

 <li>Print out the vertices on the path, in order from start to goal.</li>

 <li>Print out the length of this path and the total number of vertices visited.</li>

 <li>Devise a strategy for determining the second shortest path between the vertices.</li>

 <li>Find the second shortest path between the start and goal vertices specified in the file.</li>

 <li>Print out the vertices on the path, in order from start to goal.</li>

 <li>Print out the length of this path and the total number of vertices visited.</li>

 <li>Optimize your shortest and second shortest path algorithms to improve their performance.</li>

</ol>

The data files are constructed as follows:




<ul>

 <li>Two integers: nVertices and nEdges, the number of vertices and edges in the graph.</li>

 <li>nVertices triples consisting of the label and the x- and y-coordinates of each vertex.</li>

 <li>nEdges triples consisting of the labels of the start and end vertices of each edge, along with its weight. Note: the weight associated with an edge will be greater than or equal to the Euclidean distance between its start and end vertices as determined by their coordinates.</li>

 <li>Two labels, the indicating the start and goal vertices for which the paths are required.</li>

</ul>




A proposed solution to the second shortest path problem is as follows:




For each edge e<sub>i</sub> on the shortest path:

Find the shortest path on (V, E – {e<sub>i</sub>}).    <em>// shortest path without edge e<sub>i</sub></em> The shortest of these is the second shortest path.




<h1>Questions</h1>

<strong> </strong>

Think about this! Is this proposed solution correct always?

<ul>

 <li>What if we require that the second shortest path be longer than the shortest path?</li>

 <li>What if the graph contains cycles?</li>

 <li>What if the graph is undirected?</li>

</ul>

Explain your answers. If necessary explain how you might modify the proposed algorithm to address any issues that you identify.




Note: you may implement either the proposed solution or any modification you develop. You are not required to implement a modified proposal if you do not wish to do so.

<strong>           </strong>

<strong> </strong>

<h1>Step-1 (Week-10 demo,)</h1>

For step 1, you should read the data file into adjacency lists, or an adjacency matrix, and print on the screen the first 5 vertices and the vertices they are connected to together with their weights. e.g.:




<strong>a:  c(35)  d(27)  e(48) b:  d(35)  g(27) </strong>

<strong>c:  b(125) e(20)  f(56)  h(31)  . . . </strong>

Note: The data shown above is for format purposes only.




<h1>Step-2 (Discovering the Shortest Path)</h1>

For step 2, you should implement Dijkstra’s algorithm and find the shortest path between the start and goal vertices specified in the input file. Print out the vertices on the path (in order from start to goal), the length of this path and the total number of nodes visited by the algorithm to discover the shortest path.

<strong> </strong>

<h1>Step-3 (Discovering the Second Shortest Path)</h1>

For step 3, you should devise a strategy for determining the second shortest path between the start and goal vertices specified in the file and implement your solution. Print out the vertices on the path (in order from start to goal), the length of this path and the total number of nodes visited by the algorithm to discover the second shortest path.

<strong> </strong>

<h1>Step-4 (Optimisation)</h1>

For step 4, implement the A* algorithm and repeat Step-2 and Step-3. Print the same information to show the improved performance.

<strong> </strong>

<h1>Step-5 (Report)</h1>

In a comment block at the bottom of your program (no more than 30 lines of text) list the data structures used by your program and describe your solution to the second shortest path problem. Also, provide answer to the questions. For this step, marks will be awarded based on accuracy and correctness.

<strong> </strong>

<strong>Compilation: </strong>

All programs submitted must compile and run on banshee:

<strong>C:        gcc ass2.c  </strong>

<strong> </strong>

<strong>C++:      g++ ass2.cpp </strong>

<strong> </strong>

<strong>Java:     javac ass2.java </strong>

<strong> </strong>

<strong>Python: python ass2.py </strong>

<ul>

 <li>Programs which do not compile on banshee with the above commands will receive zero marks. It is your responsibility to ensure that your program compiles and runs correctly.</li>

</ul>