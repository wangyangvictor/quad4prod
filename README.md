In https://github.com/wangyangvictor/quad4prod/blob/main/code.txt
we present AI-generated, human-verified
[Z3Py](https://pypi.org/project/z3-solver/) code
to prove $E\le 3/2$ in Lemma 6.3 of arXiv v1 of the paper "Random Multiplicative Functions and Making Squares from Polynomial Values".
Z3Py is a Python-based implementation of Microsoft's Z3 solver,
which includes linear programming.
We ran the code online
using [Google Colab](https://colab.research.google.com/).

It is possible to explore the function $E$ further by slightly modifying the code.
For example, the equality case $E = 3/2$ can be realized even if we replace
sharp.add(R >= THREE_HALVES)
with
sharp.add(R >= 3),
but not if we replace it with
sharp.add(R >= 3.1).
