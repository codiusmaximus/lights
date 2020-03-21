# System of linear equations to solve

#### 1. Turns on red when yellow is on

#### 2.Red and green are never on together

#### 3.Blue and green can only be on and off together

#### 4.Blue and purple can not be off at the same time

#### 5.If purple is on, blue and yellow have to be on

### Equations

Let 

Y: Yellow

R: Red

G: Green

B: Blue

P: Purple



Assume a vlue of 1 as ON and 0 as OFF.

Y + R = 2

R+G=1

B-G =0

B+P  > 0 translates to - B - P < 0

P + B + Y = 3

##### Looks like this will be a MILP, as all variables can only be 1 or 0.

The system of equations can be re-written in matrix form as
$$
\left[\begin{matrix}  1&1&0&0&0\\0&1&1&0&0\\0&0&-1&1&0\\1&0&0&1&1\end{matrix}\right]\left[\begin{matrix}Y\\R\\G\\B\\P\end{matrix}\right] = \left[\begin{matrix}1\\1\\0\\3\end{matrix}\right]
$$

$$
\left[0 \ 0\ 0\ -1\ -1\right]\left[\begin{matrix}Y\\R\\G\\B\\P\end{matrix}\right]<\left[0\right]
$$

