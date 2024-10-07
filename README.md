java cProgramming Task 1: Graphs in Python [10% of your final mark]
Deadline: Sunday 6 October 2024, 23:59 Wuxi Time
This is your first programming task of this module is about graphs and implementing Dijkstra’s algorithm. You will submit a SINGLE PYTHON FILE (main.py) found in the Task1.zip file on Moodle. Your job is to modify the main.py file only. Importing any libraries that are not already imported in the main.py file is STRICTLY FORBIDDEN and will be considered as cheating.
We operate a strict zero tolerance policy on cheating and plagiarism and late penalties apply. Any deviation from the format specified above will result in you receiving the mark of zero.
THE TASK
What Are Graphs?
A weighted graph is defined as 𝐺 = (𝑁, 𝐸, 𝜆) where 𝑁 is the set of nodes, 𝐸 ⊆ 𝑁 × 𝑁 is the set of edges where (𝑛1, 𝑛2) ∈ 𝐸 if and only if (𝑛2,𝑛1) ∈ 𝐸. Finally, 𝜆: 𝐸 → N is the weighting function thatspecifiesthelengthofeachedge.Further,wehave𝜆(𝑛1,𝑛2)= 𝜆(𝑛2,𝑛1).
For example, below we have the representation of a graph 𝐺 = (𝑁, 𝐸, 𝜆) where:
• 𝑁 = {0,1,2},
• 𝐸={(0,1),(1,0),(1,2),(2,1)},
• 𝜆(0,1) = 𝜆(1,0) = 3 and 𝜆(1,2) = 𝜆(2,1) = 4.
What is an adjacency matrix?
An adjacency matrix of a weighted graph 𝐺 = (𝑁, 𝐸, 𝜆) is a |𝑁| by |𝑁| matrix 𝑚 such that 𝑚𝑖𝑖 = 0 for 𝑖 < |𝑁| and for 𝑖 < 𝑗 < |𝑁| we have
           0
3
1
4
2
   𝜆(𝑖,𝑗) 𝑖𝑓 (𝑁 ,𝑁 ) ∈ 𝐸 𝑖𝑗
m𝑖𝑗 = {
∞ 𝑜𝑡h�代 写program、python
代做程序编程语言�𝑟𝑤𝑖𝑠𝑒
For example, the graph above has the below adjacency matrix:
03∞ 𝑚=(3 0 4)
∞40

Your Python Implementation
Open the main.py file from Task1.zip. THIS IS THE ONLY FILE YOU SHOULD CHANGE ANF UPLOAD TO MOODLE. ONLY UPLOAD THIS FILE AND DO NOT ADD ANY NEW IMPORT STATEMENTS TO IT. In order to test your score, simply run the main.py file.
(1) In order to obtain the first five marks:
Usingtheinf importedfrommath,modifythe__init__,addEdge,andgetAdjacencyMatrix methods so that the initialisation method creates a graph with noOfNodes nodes, assume they are called [0, 1, ..., noOfNodes-1] and no edges. The addEdge method adds an edge between x and y of length weight. For example, you would write the below code to create the graph on the previous page.
And then the below code
g.getAdjacencyMatrix() would result in
[[0, 3, inf], [3, 0, 4], [inf, 4, 0]]
(2) In order to obtain the second five marks:
Modify the shortestRoute method so that it returns a dictionary with the key distance corresponding to the value of the total distance of the shortest route between the nodes x and y and the key path corresponding to the nodes in that route in order. You may find it useful to search for Dijkstra’s algorithm. For example, the g.shortestRoute(2,0) call for the g above would result in:
{"distance":7, "path":[2,1,0]}
     g = Graph(3)
 g.addEdge(0,1,3) g.addEdge(1,2,4)
    
         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
