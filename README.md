[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

**Firstly, the definition of big O is $f(n)\in o(g(n)) \iff \exists c>0, \exists n_0 \in N : \forall n\ge n_0, |f(n)| \le c * |g(n)|$**

**To prove that $f(n)\in o(g(n))$ implies $f(n)\in O(g(n))$, we must show that for any two functions f(n) and g(n) such that $f(n)\in o(g(n))$, there exist constants c' and $n_0$' such that f(n) $\le$ c'g(n) $\forall$ n $\ge$ $n_0$'**

**So, given that $f(n)\in o(g(n))$, we know that $\forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$.**

**We can choose c' = c and $n_0$' = $n_0$, which means that $\forall n \ge n_0', f(n) < cg(n)$, which implies that $f(n) \le cg(n).$**

**Therefore, $f(n)\in O(g(n))$, and thus we can conclude that $f(n)\in o(g(n))$ implies $f(n)\in O(g(n))$.**
