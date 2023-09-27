A mathematical way to represent a system of [[Logic gates]]
# Syntax
A bar on top is not,
. is AND
\+ is OR
$\oplus$ is XOR
# Identities
$$ A . 1 = A$$
$$A.0=0$$
$$A.A=A$$
$$A.\overline{A}=0$$
$$A + 1 = 1$$
$$A + 0 = A$$
$$A+A = A$$
$$A+\overline{A} = 1$$
$$A + \overline{A}.B = A + B$$
$$A.B + A = A.(B+1) = A$$


An Example truth table looks like the following:

| C   | B   | A   | Q   | Equation                      |
| --- | --- | --- | --- | ----------------------------- |
| 0   | 0   | 0   | 0   | 3                             |
| 0   | 0   | 1   | 1   | $\overline{C}.\overline{B}.A$ |
| 0   | 1   | 0   | 0   |                               |
| 0   | 1   | 1   | 1   | $\overline{C}.B.A$            |
| 1   | 0   | 0   | 1   | $C.\overline{B}.\overline{A}$ |
| 1   | 0   |     | 1   | $C.\overline{B}.A$            |
| 1   | 1   | 0   | 0   |                               |
| 1   | 1   | 1   | 0   |                               |

We can generate an expression for the table by 'OR' each term together

$$Q = \overline{C}.\overline{B}.A+\overline{C}.B.A + C.\overline{B}.\overline{A} + C.\overline{B}.A $$
This can be simplified by Factoring out common terms

$$Q=\overline{C}.A. (\overline{B}+B) + C.(\overline{B}.\overline{A} + \overline{B}.A)$$
Then using identity $A+\overline{A}=1$ we can say that
$$Q=\overline{C}.A.(1) + C.\overline{B}$$
