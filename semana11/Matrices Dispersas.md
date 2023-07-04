## Matrices Dispersas


set(i, j, data):
- verificar que i, j no excedan nxm
- temp = matrix[i]
- repetir mientras j > temp.col
  - si j == temp.col, temo.data = data
  - si j < temp.col, insertar nuevo nodo antes de temp.col
  - si se inserta en el primer nodo, se actualiza el puntor en el array matrix
 
### ELIMINACION

La eliminacion no cambia en la resolucion de la matriz


### Suma de matrices

sumaMatrices(M1, M2)
for(i=0 ... n-1)
  1m = merge(M1, get)
