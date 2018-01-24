# intro to BLAS

## HowTo with blas level 1 

   **Swap two vectors:** `v1` and `v2` of size `s`, and 
   `spc` as storage space between elements

```fortran
sswap( s, v1, spc1, v2, spc2 )
dswap( s, v1, spc1, v2, spc2 )
zswap( s, v1, spc1, v2, spc2 )
```

   **Copy one vector:** `v1` to `v2` of size `s`
   
```fortran
scopy( s, v1, spc1, v2, spc2 )
dcopy( s, v1, spc1, v2, spc2 )
zcopy( s, v1, spc1, v2, spc2 )
```

   **Scale one vector:** `v1` by `alpha` of size `s`
   
    <img src="https://latex.codecogs.com/gif.latex?O_t=\text { Onset event at time bin } t " />
    
```fortran
sscal( s, alpha, v1, spc1 )
dscal( s, alpha, v1, spc1 )
zscal( s, alpha, v1, spc1 )
```