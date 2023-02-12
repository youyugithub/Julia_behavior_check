# Julia_behavior_check

## When can matrices be reduced to vectors 
```
A=[1 2;3 4]
A[1,:]
# vector
A[1:1,:]
# matrix
A[[1],:]
# matrix
```

```
A=Matrix{Vector}(undef,4,4)
A[1,1]=[1]
B=[1 2;3 4]
B[A[1,1],:]
# matrix of one row
```
