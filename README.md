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

