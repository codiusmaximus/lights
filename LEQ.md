### Carousel lights problem solution via Linear Equations

#### Bhaskar Agarwal

The rules for the 5 switches are the following. All 5 are turned on simultaneously.

1. Turns on red when yellow is on
2. Red and green are never on together

3. Blue and green can only be on and off together

4. Blue and purple can not be off at the same time

5. If purple is on, blue and yellow have to be on

### Equations

Let Y: Yellow , R: Red , G: Green , B: Blue , P: Purple. Assume a vlue of 1 as ON and 0 as OFF.

$Y - R \leq 0$  (cond. 1)

$R+G\leq1$ (cond. 2)

$B-G=0$ (cond. 3)

$-B-P\leq-1$ (cond. 4)

$P -B - Y \leq -1$ (cond. 5 maybe this works)

$-Y-R-G-B-P \leq -1$ 
(Additional condition meaning they all can not be off)

##### Looks like this will be a MILP, as all variables can only be 1 or 0.

The system of equations can be re-written in matrix form as
$$
\left[\begin{matrix}  0&0&-1&1&0\end{matrix}\right]\left[\begin{matrix}Y\\R\\G\\B\\P\end{matrix}\right] = \left[\begin{matrix}0\end{matrix}\right]
$$

$$
\left[\begin{matrix}1&-1&0&0&0\\0&1&1&0&0\\0&0&0&-1&-1\\-1&0&0&-1&1\\-1&-1&-1&-1&-1\end{matrix}\right]\left[\begin{matrix}Y\\R\\G\\B\\P\end{matrix}\right]\leq\left[\begin{matrix}0\\1\\-1\\-1\\-1\end{matrix}\right]
$$

#####These equations successfully solve the problem.

