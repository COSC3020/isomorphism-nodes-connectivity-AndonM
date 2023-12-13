[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11974292&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

INSPIRATION TAKEN FROM CADE MAYNARD

Because we know our graphs $A$ and $H$ have the same number of nodes and are completely connected, we can deduce that there exists a bijective function that maps one to the other and that every node in both graphs will have the same amount of edges compared to every other node in their respective graphs. By extensions, we may also conclude that every node in our first graph $(G_1)$ must have the same number of edges as every node in our second graph. $(G_2)$ With this in mind, if we map a vertex in $G_1$ to a vertex in $G_2$ we see that every edge connected to our $G_1$ vertex will map to an edge connected to the mapped vertex in $G_2$. As a consequence of this, any mapping with no repetition from each node in $G_1$ to $G_2$$ will be bijective. One particular function that maps from one graph to the other can be constructed by taking an arbitrary permutation of every node from $G_1$ and an arbitrary permutation of every node from $G_2$. From here, take each node from our $G_1$ permutation and map it to a node in our $G_2$ permutation. This creates a bijective mapping from $G_1$ to $G_2$ proving an isomorphic relationship between $G_1$ and $G_2$.
