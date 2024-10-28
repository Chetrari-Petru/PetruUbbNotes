12
We have the following affirmations
$$
\begin{align}
&A: \text{This afternoon is sunny} \\
&B: \text{It is colder than yesterday} \\
&C: \text{We will go swimming} \\
&D: \text{We will take a canoe trip} \\
&E: \text{We will be home by sunset} \\
\end{align}
$$
And the following propositions
$$
\begin{align}
&H_{1}: \lnot A \land B \\
&H_{2}: A \to C \\
&H_3 : \lnot C \to D \\
&H_4 : D \to E
\end{align}
$$

Building the eaxiomatic system
$$
\begin{align}
&f_1 =  H_{1} \\
&f_{2} = H_{2} \\
&f_{3} = H_{3} \\
&f_{4} = H_{4} 
\end{align}
$$

So now to try and build a deduction
$$
\begin{align} 
&f_{1}\phantom {,f_{1}} \vdash \lnot  A:f_{5} \\
&f_{5}, f_{2} \vdash_{mp} \lnot C :f_{6} \\
&f_{3}, f_{6} \vdash_{mp} D : f_{7} \\
&f_{4},f_{7} \vdash_{mp} E :f_{8}
\end{align}
$$
so we got to the logical conclusion that "we will be home by sunset" and we can say that
the sequence of formulas $(f_{1},f_{2},f_{3},f_{4},f_{5},f_{6},f_{7},f_{8})$ is the deduction of  $E$ from the hypothesis
so $\text{We will be home by sunset}$


**Prove me wrong**
