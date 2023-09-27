Used to simplify linear circuits into an equivalent circuit with a single ideal [[Voltage]] source and a single ideal [[Resistors|resistor]] in series.

Given the following circuit
![[Potential Divider 1.png]]
We can calculate the open circuit voltage, short circuit current and equivalent resistance.

$$\mathbf V_{oc} = \frac{R_2}{R_1 + R_2} \times V_{in}$$
$$V_{oc} = \frac{1.8\text{k}}{1.2\text{k}+ 1.8\text{k}} \times 9 = 5.4\text{V}$$

$$I_{sc} = \frac{V_{in}}{R_1} = \frac{9}{1.2\text{k}} = 0.75\text{mA}$$
$$R_{eq} = \frac{V_{oc}}{I_{sc}} = \frac{5.4\text{V}}{0.75\text{mA}} = 0.72\text{k}\ohm$$
Combining these into the equivalent circuit gives:
![[Equivalent Circuit.png]]