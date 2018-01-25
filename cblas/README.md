# Intro to BLAS

## HowTo with blas level 1 

   **Swap two vectors:** `v1` and `v2` of size `s`, and 
   `spc` as storage space between elements

   `tmp = v1; v1 = v2; v2 = tmp;`

```fortran
sswap( s, v1, spc1, v2, spc2 )
dswap( s, v1, spc1, v2, spc2 )
zswap( s, v1, spc1, v2, spc2 )
```

   **Copy one vector:** `v1` to `v2` of size `s`

   `v2 <= v1;`

```fortran
scopy( s, v1, spc1, v2, spc2 )
dcopy( s, v1, spc1, v2, spc2 )
zcopy( s, v1, spc1, v2, spc2 )
```

   **Scale one vector:** `v1` by `alpha` of size `s`
   
   `v1 = alpha*v1;`
    
```fortran
sscal( s, alpha, v1, spc1 )
dscal( s, alpha, v1, spc1 )
zscal( s, alpha, v1, spc1 )
```

   **Scale one vector add another vector:** `v1` by `alpha` plus `v2`
   
   `v2 = alpha*v1+v2;`
    
```fortran
saxpy( s, alpha, v1, spc1 , v2, spc2 )
daxpy( s, alpha, v1, spc1 , v2, spc2 )
zaxpy( s, alpha, v1, spc1 , v2, spc2 )
```

   **Find the index i of the max element:** `v1[i]` is one of the higher values of `v1`
   
   `i = argmax_i(v1);`
    
```fortran
isamax( s, v1, spc1 )
idamax( s, v1, spc1 )
izamax( s, v1, spc1 )
```

   **norm 2:** `|v1|` norm-2
   
   `|v1|_2 = norm2(v1);`
    
```fortran
snrm2( s, v1, spc1 )
dnrm2( s, v1, spc1 )
znrm2( s, v1, spc1 )
```

   **norm sum:** `|v1|` norm-1
   
   `|v1|_1 = norm1(v1);`
    
```fortran
sasum( s, v1, spc1 )
dasum( s, v1, spc1 )
zasum( s, v1, spc1 )
```
