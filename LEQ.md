# System of linear equations to solve

### Lights problem

#### Bhaskar Agarwal

The logic for the lights is the following

1. Turns on red when yellow is on

2.Red and green are never on together

3.Blue and green can only be on and off together

4.Blue and purple can not be off at the same time

5.If purple is on, blue and yellow have to be on

### Equations

Let Y: Yellow , R: Red , G: Green , B: Blue , P: Purple. Assume a vlue of 1 as ON and 0 as OFF.

Therefore

Y + R = 2 (cond. 1)

R+G=1 (cond. 2)

B-G =0 (cond. 3)

B+P  > 0 translates to - B - P < 0 (cond. 4)

P + B + Y = 3 (cond. 5) THIS IS WRONG- NEEDS WORK

##### Looks like this will be a MILP, as all variables can only be 1 or 0.

The system of equations can be re-written in matrix form as
$$
\left[\begin{matrix}  1&1&0&0&0\\0&1&1&0&0\\0&0&-1&1&0\\1&0&0&1&1\end{matrix}\right]\left[\begin{matrix}Y\\R\\G\\B\\P\end{matrix}\right] = \left[\begin{matrix}1\\1\\0\\3\end{matrix}\right]
$$

$$
\left[0 \ 0\ 0\ -1\ -1\right]\left[\begin{matrix}Y\\R\\G\\B\\P\end{matrix}\right]<\left[0\right]
$$

