Shapes.

## Set Theory 

- Union
- Intersect 
- Negate
- Reflection, $\hat{A}$

- Boundary detection
- Region filling
- Extraction

- Convex hull: outline
- Thinning: shrink shape
- Thickening: expand shape
- Skeleton: get structure
- Pruning: kill minor branches for thinning and skeleton
- 

## Dilation & Erosion

Let a square $A$ with sides $x$, and dilation of $A$, $\hat{A}$ is $x/4$ for each sides. 

- Each sides of $A$ will grow by a factor of $\hat{A}/2$, which is $x/8$ each sides.

## Opening & Closing

- Opening: erosion then dilation, kill spots
- Closing: dilation then erosion, fill gaps

## Hit-or-Miss Transformation [^1]

- Dilation & Erosion ++ 
- Detect shapes



## References

[^1]: https://homepages.inf.ed.ac.uk/rbf/HIPR2/hitmiss.htm
