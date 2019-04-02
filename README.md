# Ipv6Finder

Crawls IPV6 in websites.

## Expressão Regular
```
    ([0-9aA-fF]{1,4}:){1,7}([0-9aA-fF]{1,4})
```

## Gramática

```
S -> [0-9X]A
A -> [0-9X]B | :E
B -> [0-9X]C | :E
C -> [0-9X]D | :E
D -> :E

E -> [0-9X]F
F -> [0-9X]G | :J
G -> [0-9X]H | :J
H -> [0-9X]I | :J
I -> :J

J -> [0-9X]K
K -> [0-9X]L | :O
L -> [0-9X]M | :O
M -> [0-9X]N | :O
N -> :O

O -> [0-9X]P
P -> [0-9X]Q | :T
Q -> [0-9X]R | :T
R -> [0-9X]S | :T
S -> :T

T -> [0-9X]U
U -> [0-9X]V | :Y
V -> [0-9X]W | :Y
W -> [0-9X]X | :Y
X -> :Y

Y -> [0-9X]Z
Z -> [0-9X]A1 | :D1
A1 -> [0-9X]B1 | :D1
B1 -> [0-9X]C1 | :D1
C1 -> :D1

D1 -> [0-9X]E1
E1 -> [0-9X]F1 | :I1
F1 -> [0-9X]G1 | :I1
G1 -> [0-9X]H1 | :I1
H1 -> :I1

I1 -> [0-9X]J1 
J1 -> [0-9X]K1 
K1 -> [0-9X]L1 
L1 -> [0-9X]M1 
M1 -> λ
```