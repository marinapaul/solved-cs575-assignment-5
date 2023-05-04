Download Link: https://assignmentchef.com/product/solved-cs575-assignment-5
<br>
<strong><u>Objective: </u></strong>

<ul>

 <li>Enhance the concept of greedy algorithms</li>

 <li>Design program for greedy algorithm implementation.</li>

</ul>

<u>Part A </u>

<ol>

 <li> Find the minimum spanning tree using the Prim’s algorithm for the following graph starting at node A. Show the order that the nodes are added into the minimum spanning tree. Draw the minimum spanning tree and indicate the weight summation of the MST.</li>

</ol>

[<strong>Optional programming: extra 8%]</strong> Implement the algorithm and print out the MST by your program.

<ol start="2">

 <li> Suppose that we have an international conference, and need to schedule a series of sessions among a number of hotel conference rooms. We wish to schedule all the sessions using as few rooms as possible for saving budget. For example: we need to schedule following sessions:</li>

</ol>

Session 1 (Education): at 9:30 – 10:30am

Session 2 (Economics): at 9:30 – 10:30am

Session 3 (Security):  at  1:30 – 2:30pm

Session 4 (Med-Care):   at 12:00 –1:00pm

Session 5 (Insurance):  at 10:30 – 11:30am

Session 6 (Science):  at 11:30am – 12:30pm

Section 7 (Technology):  at  11:30am  – 12:30pm

Session 8 (Transportation):  at 1:00 – 2:00pm

Give an efficient greedy algorithm to determine how many conference rooms are needed. Show your solution and discuss whether your algorithm could always generate the optimal solution. What is the time complexity if k rooms are needed.




<ol start="3">

 <li> Explain that if there is one edge with a weight smaller than all the other edges, that edge will be part of every minimum spanning tree.</li>

 <li> Explain whether it is always, never, or sometimes true that the order in which the nodes are added to the MST by the Prim algorithm is the same as the order in which they encountered in the breadth-first search.</li>

 <li>(1)  Suppose there are a group of cities, which are modeled by a strongly connected undirected graph G = (V, E) with positive edge weights representing the distances between two cities. A particular city is the capital city a Î Design an efficient algorithm for finding shortest paths between all pairs of cities, with the one restriction that these paths must all pass through the capital city. (Note that: we allow one city to be passed more than once if needed). Show the shortest path from node <em>d</em> to node <em>i</em> via node <em>a. (</em>Suppose the capital city is node “<em>a</em>”).</li>

</ol>

(2)<strong> (Optional programming: extra 8%)</strong> Implement your designed algorithm, and print out the shortest path of all the pairs via node <em>a</em> using the following graph. Suppose the capital city is node “<em>a</em>”.

<ol start="6">

 <li> Suppose the Dijkstra’s algorithm runs on the following graph, starting at node A. (a) Draw a table showing the intermediate distance values of all the nodes at each iteration of the algorithm. (b) Show the final shortest-path tree.</li>

</ol>




<ol start="7">

 <li> To construct a road network, we need to plan a minimum cost. Using Kruskal’s algorithm to find your solution. You don’t need to show every step. But you need to show the final result and the disjoint sub-sets in the intermediate step when the edge (e, i) is selected.</li>

</ol>




<ol start="8">

 <li> You are downloading <em>n</em> files (songs, programs) from the web to a minimum number of CDs. Each CD can store exactly B bytes. More than one file can be stored on each CD, but a single file cannot be stored on more than one CD (no split).  Each file <em>i</em> has a size <em>s</em><sub>i</sub> bytes (<em>s</em><sub>i</sub> £B). Describe a greedy algorithm to solve this problem. It may not get optimal solution, If so, give a counter example.</li>

</ol>

<strong> </strong>

<ol start="9">

 <li>The notion of a minimum spanning tree is applicable to a connected weighted graph. Do we have to check a graph’s connectivity before applying Prim’s algorithm or can the algorithm do it by itself? Explain your answer.</li>

 <li> Design an algorithm for finding a maximum spanning tree – a spanning tree with the largest possible edge weight–of a weighted connected graph.</li>

</ol>

<strong> </strong>

<strong>Part B:</strong>

<strong> </strong>

<ol>

 <li><strong> Programming</strong></li>

</ol>

Objects classification is one of the important tasks for pattern analysis. For example, clustering objects with similar shapes or colors to create a database with a number of object categories. In this assignment, you are required to design an algorithm by using the concept of disjoint set to classify a set of objects into a number of categories.




<ol start="100">

 <li>The similarity between a pair of objects is measured by a value in the range from 0 to 100. You can sort the similarity in a non-increasing order. <strong><em>(Note: The higher value, the higher similarity between two objects).</em></strong></li>

 <li>Given a set of objects and the similarity between any pair of objects, design an algorithm for finding a number of disjoint sub-sets, which means you need to create a number of maximum spanning trees instead of a single spanning tree. Each category is a single maximum spanning tree. (note that we call it “maximum” because we hope to create a spanning tree with maximum similarity).</li>

</ol>




<ol>

 <li>Suppose the number of categories is known, solve the following problem:</li>

</ol>




<strong> Problem:</strong> There are 20 photos with three categories (i.e., trees, animals, buildings). Assume photos within a same category have more similarity than the photos in different categories. Classify 20 photos G= (p1, p2, p3, …, p20) into three disjoint sub-set, and print out the number of photos in each sub-set and the IDs of photos in each sub-set.




39 edges are given below, which correspond to the similarities between two photos:




S(p1, p2) = 80;

S(p5, p9) = 73;

S(p9, p13) = 69;

S(p2, p3) = 10;

S(p5, p7) = 20;

S(p5, p2) = 74;

S(p9, p18) = 15;

S(p13, p14) = 21;

S(p9, p1) = 92;

S(p13, p2) = 59;

S(p20, p4) = 6;

S(p18, p17) = 17;

S(p11, p3) = 74;

S(p7, p18) = 83;

S(p7, p12) = 27;

S(p1, p10) = 16;

S(p5, p15) = 47;

S(p20, p14) = 94;

S(p14, p18) = 77;

S(p2, p4) = 30;

S(p11, p14) = 62;

S(p3, p20) = 85;

S(p11, p7) = 62;

S(p6, p10) = 87;

S(p12, p15) = 81;

S(p3, p19) = 39;

S(p9, p8) = 45;

S(p19, p4) = 65;

S(p8, p16) = 70;

S(p15, p17) = 64;

S(p1, p11) = 32;

S(p11, p6) = 43;

S(p12, p6) = 87;

S(p12, p19) = 70;

S(p7, p16) = 39;

S(p13, p6) = 22;

S(p4, p16) = 68;

S(p17, p10) = 56;

S(p19, p15) = 71.