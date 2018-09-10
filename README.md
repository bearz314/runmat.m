# runmat.m
Create a matrix with consecutive numbers of given dimension

## Usage
For temporary use, put it in your working directory. For a more permanent use, put it in a folder and include it in `HOME > ENVIRONMENT > Set Path`. This script can thus be used without having it in the working directory. (Obviously, calling this function on another computer without this `m` file will not work.)

## Syntax
```
A = runmat(sz)
A = runmat(sz1,...,szN)
```

## Description
* `A = runmat(sz)` creates a matrix of running matrix with size `sz-by-sz`.
* `A = runmat(sz1,...,szN)` creates a matrix of running matrix with size `sz1-by-...-by-szN` array.

## Examples

### Example 1
Create a 5-by-5 matrix.
```
A = runmat(5)
```

```
A =

     1     2     3     4     5
     6     7     8     9    10
    11    12    13    14    15
    16    17    18    19    20
    21    22    23    24    25
```

### Example 2
Create a 2-by-3-by-2 matrix.
```
A = runmat(2,3,2)
```

```
A(:,:,1) =

     1     2     3
     4     5     6


A(:,:,2) =

     7     8     9
    10    11    12
```
