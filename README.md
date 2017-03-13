# grafikz

##0216
- Using EDGE LISTS: a list of points where every 2 points represent endpoints of a line
 - ex: triangle ABC: [A,B,B,C,C,A]
 - implement some routine: every 2 points, call drawline
 - facilitate transformation
- storing/representing edge lists:
 - each point: THREE numbers, x y z (thinking ahead!)
 - each component should be a floating point.. bc scaling could involve float
 - and... a 1.0. so (FOUR NUMBERS) x, y, z, 1.0
```
x0 x1 xn
y0 y1 yn
z0 z1 zn
1.0 1.0 1.0
```
- it's a matrix! transformations!!!  
- matrix math
  - scalar mult
   - s * [ a b | cd ] = [ sa sb | sc sd ]
  - matrix mult
   - (M)(N) 
   - # col M = # row N
   - (AxB)(BxC) = AxC
   - we will always have (4xN) edge
   - (4x4)(4xN) = (4xN) but why (4x4)?
- multiplicative identity

###0309

double stop = 1.001; //buffer for imprecise floatin
for (t=step; t<=stop; t+=step)
###0310
lost note
###0313
bezier curves 
- linear BC `P(t) = (1-t)*P0 + t*P1`
- quadratic BC `Q(t) = (1-t)^2P0 + 2t(1-t)P1 + t^2*P2`
- BINOMIAL EXPANSION-LIKE COEFFICIENTS
- but... we want at^3 + bt^2 + ct + d
```
Bezier matrix:
-1 3 -3 1
3 -6 -3 0
-3 3 0 0
1 0 0 0
x
Input matrix:
P0
P1
P2
P3
=
Coeffficients
a
b
c
d
```
