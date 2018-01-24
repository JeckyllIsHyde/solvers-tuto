# intro to BLAS

## HowTo with blas level 1 
   Swap two vectors `v1` and `v2` of size `s`:
   `spc` as storage space between elements

```fortran
sswap( s, v1, spc1, v2, spc1 )
```