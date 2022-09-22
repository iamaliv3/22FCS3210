# Left Recursion Elimination

Eliminate any left-recursive productions (including indirect ones). When you are done, submit this README.md file with your answers on Canvas. 

## Q1

```
X -> XYz | Xw | w
Y -> Yp | q

X -> wX'
X' -> YzX'| wX'| eps 

Y -> qY'
Y' -> pY'| eps

```
## Q2

```
S -> aA | Sd
A -> b
replace A
S-> ab | Sd
S -> abS'
S' -> dS' | eps
```

## Q3

```
A -> Bxy | x
B -> CD
C -> A | c
D -> d    

replacing D
A -> Bxy | x
B -> Cd
C -> A | c

replacing C
A -> Bxy | x
B -> Ad | c 

replacing B
A -> Adxy |c|x

A -> cA' | xA'
A' -> dxyA' | eps
```
