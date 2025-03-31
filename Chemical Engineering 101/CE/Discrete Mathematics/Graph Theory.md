Diagonal Subset : $\Delta(V) = \{(v,v)\mid v\in V\} \subseteq V \times V$
Undirected Graph : $(v_i, v_{j\neq i})=(v_j, v_{i\neq j})$
Directed Graph : $(v_i, v_{j\neq i})\neq(v_j, v_{i\neq j})$

$T = (V,E)$
$\Phi = V,$ assume: $|V|<\infty$
$E\subseteq \mathcal{P}_2(V) = \{A\subseteq V\big|\mid A \mid =2\}$

$u\in V;\ \deg(u) :=\{e\in E | u\in e\}$
$\forall u \in V,\ 0\leq\deg(u)\leq n-1$

if $v_i\neq v_j,$ then $\deg(v_i) \neq \deg(v_j)$
is False
Implies
$\exists v_i,v_j\in V$ s.t. 
1. $v_i \neq v_j$
2. $\deg(v_i) = \deg(v_j)$

## Isomorphism

$\Gamma_1,\Gamma_2 =$ graphs
$\Gamma_1\cong \Gamma_2 \implies\Gamma_1$ is isomorphic to $\Gamma_2$ 
if $f: V(\Gamma_1)\to V(\Gamma_2)$
1. $f$ is a bijective function
2. $\{v_i,v_j\}\in E(\Gamma_1) \iff \{f(v_i),f(v_j)\}\in E(\Gamma_2)$
3. $\deg(v_i)=\deg(f(v_i))\forall i \in \{1,\ldots,n\}$

## Regular Graphs
Given $v_i,v_j \in V$
$\deg(v_i) = \deg(v_j)$
$\deg:V\to \{0,\ldots n-1\}$ is a constant function
$\forall v \in V, \deg(v) = n-1$ Complete Graph























