# ¿Ques es un grafo?


es un par de conjuntos finitos entre vertices y aristas.

V = {A, B, C, D, E, ...} denota los vertices
E = {{A, B}, {A, C}, ...} denota entre que vertices hay una arista

- Pueden existir dos caminos entre dos vertices

## Grafo no direccionado o no dirigido

Se cumple la propiedad de: {a, b} = {b, a}

## Para grafos dirigidos

Notacion: {(A, B), (B, C), ...}

## Grafo Ciclico y grafo aciclico

- Si contiene ciclos entonces es ciclico
- Un arbol es un grafo aciclico


## Notas:
- 


# Arbol

- Es un tipo especial de grafo donde se tiene un nodo raiz y una relacion de paternidad entre nodos
- la cantidad de aristas es igual a la cantidad de vertices - 1

## Propiedades:

### Adayacencia:
Si dos vertices xi y xj estan conectados por una arista son adyacentes
### Incidencia: 
una arista es incidente a sus vertices
### Grado: 
El numero de aristas incidentes a un vertice, es su grado.
- Un vertice aislado tiene grado 0
- un vertice hoja tiene grado 1

## Grafo completo
Es un grafo 100% lleno con un maximo de aristas


## seudocodigo 
G = (V, E)   

V = (a, b, c, d)
### Dirigido
-----------------------------------------
a => (a, b) (a, c) (a, d)... 3
b => (b, a) (b, c) (b, d)... 3
c => ....................... 3
d => ....................... 3
Total: 12

max E => V*(V-1)

### No-Dirigido
---------------------------------------
a => (a, b) (a, c) (a, d) ... 3
b => (b, c) (b, d) .......... 2
c => (c, d) ................. 1
d => ........................ 0
Total: 6

max E => V*(V-1)/2

## Densidad de un grafo


## Codigo:

struct Edge{
  string startVertex;
  string endVertex;
  float wight;
}

class Graph{
  vector<string> vertex;
  vector<Edge*> edges;
}

### Representacion ingenua

Espcio: O(V) + O(E)
Cuanto toma encontrar los nodos adyacentes a un nodo: V*(V-1)

  
### Representacion de grafos
- Por Matriz de Adyacencia:
- 

#### Matriz de Adyacencia
  matriz de nxn donde n = V
  
