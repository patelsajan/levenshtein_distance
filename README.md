the Levenshtein distance (also called edit distance) is a number that tells how different two strings are. the higher the number, the more different two strings are.

the levenshtein distance between two string a,b of length |a| and |b| respectively is given by lev(a,b) where

```math
lev(a,b)=\begin{cases}|a| & if |b| = 0\\|b| & if |a| = 0 \\lev(tail(a), tail(b)) & if a[0] = b[0]\\1+min\begin{cases}lev(tail(a), b)\\lev(a, tail(b))\\lev(tail(a), tail(b) \end{cases} & otherwise,\end{cases}
```

where the tail of some string x is a string of all but the first character of x, and x[n] is the nth character of the string x. counting from 0.


