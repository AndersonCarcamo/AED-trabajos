# Disjoint Sets

Conuntos Disjuntos:

Sea:
A = {a, b, c, d}
B = {x, y, z}
C = {h, i, j}

find(c) = A
union(x, d) = find(x) U find(A)
            = {x, y, z, a, b, c, d}
------------------------------
usando arrays
find(x) ===> o(n)
union(x, d) ==> O(n) + O(n) + O(n)
-------------------------------
usando listas
find(c) ==> O(n)
union(x, d) ==> O(n) + O(n) + O(1)
-------------------------------
usando avl (con todos los elementos)
find(c) ==> O(log(n))
union(x, d) ==> O(log(n)) + O(log(n)) + O(n)
-------------------------------
usando avl por cada conjunto
find(c) =>
union(x, d) =>
-------------------------------

usando hash con todos los elementos
A = {a, b, c, d}
B = {c, y, z}
C = {h, j, k}

hashtable = {(a:A}, (b, A), (c: A), ..., (x:B), (y:B), ..., (h:C)}
find(c) = O(1)
union(x, d) => O(1) + O(1) + O(n)


-----
find(c) ==> O(k), O(1)
union(x, d) ==> find + O(1)

## OPERACIONES

### FIND

function Find(x)
  if x, parent == x
    return x
  else
    return, parent := yRoot

### UNION

function Union(x, y)
  xRoot := Find(x)
  yRoot := Find(y)
  

### OPTIMIZACION

funciton Union(x, y)
  xRoot := Find(x)
  yRoot := Find(y)
  if xRoot == yRoot
    return
  if xRoot.rank < yRoot.rank
    xRoot.parent := yRoot
  else if xRoot.rank
  
  
### KRUSKAL
Funciona dependiendo del calculo del peso minimo de las aristas.
Seudocodigo:

Analiza los pesos de las aristas conexas al vertice de inicio
Selecciona el de menor costo y vuelve a analizar el de menor costo.
Si la arista ya esta conectada a un vertice pasado, no se toma y si ya no hay vertices para tomar, se toma como completado el sistema
