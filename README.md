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

I WASN'T SURE HOW TO WRAP IN MATHEMATICAL NOTATION INTO THIS

Suppose two graphs A & B are not isomorphic, meaning there is no bijective function between their nodes that preserves adjacency relationships. Since A and B have the same number of nodes n, there must be some node in A that does not have a corresponding node in B under this assumption. Focusing on this unmatched node in A, we know this node is connected to every other node in A by the definition of a completely connected graph. However, since there is no corresponding node in B, this means that B cannot have a node that is connected to all nodes in B which contradicts the definition of a complete graph. Again, by the definition of a complete graph, every node is connected to every other node. Therefore, B must have a node that is connected to all the nodes in B. However, if B, has a node that is connected to all nodes in B, and A and B have the same number of nodes, this node must have a corresponding node in A leading to our contradiction of there being an unmatched node in A. Because the contradiction arose from our intioal assumption that A and B are in fact not isomorphic, we have shown A and B to in fact be isomorphic by contradiction.
