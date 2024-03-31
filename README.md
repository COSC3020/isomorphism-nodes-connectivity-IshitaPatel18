[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/ppBU16qM)
# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Proof: Suppose that $G_1$ and $G_2$ are graphs that have the same number of nodes and are
completely connected which means every node shares an edge with every other node in the graph.
For $G_1$ and $G_2$ to be isomorphic, there must exist a bijection function which means a 
one-to-one and onto function exists. A one-to-one function exists, if there are distinct 
vertices from $G_1$ that map to distinct vertices in $G_2$. An onto function exists, if it 
is possible to trace all vertices in $G_2$ to a vertex in $G_1$. A bijection function leads 
to a one-to-one correspondence, or a pairing of vertices essentially. Since both graphs have 
the same number of nodes, it is possible to map each node in $G_1$ to a node in $G_2$. If both 
graphs have different number of nodes, then they would not be isomorphic as shown by the 
isomorphism-nodes exercise, which shows that if two graphs don't share the same number of 
nodes either a one-to-one or an onto function will not be possible, so a bijection fuction is out 
of reach. Since both graphs are fully connected, for n number of nodes, there will be n-1 edges from
each node, connecting to the rest of the nodes. Now, since every node is connected to every 
other node, each node from $G_1$ can be randomly paired with a unique node in $G_2$. Since both 
graphs are completely connected, it wouldn't matter what nodes were paired as each paired node 
will have an edge that connects to every other node, so the corresponding edges will be maintained 
in both graphs, regardless of the permutation. This means that any permutation of the mapping of the 
vertices would allow a one-to-one and onto function as no two nodes from $G_1$ will map to one 
node in $G_2$ and all nodes from $G_2$ can be traced to a node in $G_1$. Also, the edges connecting 
any two nodes in $G_1$ and $G_2$ will also be maintained when vertices of $G_1$ are mapped to 
$G_2$ because there exists an edge between any two nodes in both graphs. Any permutation will allow a 
bijection function to map all vertices from $G_1$ onto $G_2$, where all corresponding edges will be maintained. 
Therefore, if $G_1$ and $G_2$ have the same number of nodes and are completely connected, they must be isomorphic. 

Sources: The Introduction to Algorithms textbook, pages 1161, 1161, and 1166
