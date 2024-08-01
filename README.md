# Reto-10
1. Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.
````python
#Cree una lista vacia para almacenar los datos
nums = []
print("¿cuántos números ingersará?")
n = int(input())
i = 0
#Cree un ciclo para que el usuario digite los números a ingresar
while i < n:
    print("valor número: ",i+1)
    val = float(input())
    nums.append(val)
    i+=1
#Cree una función para hallar el promedio de la lista
prom = sum(nums) / len(nums)
print( "El promedio es: ",prom)
````
2.Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.
```python
Lista1 = [1,2,3,4]
Lista2 = [4,3,2,1]
Producto : int = 0
for i in range(len(Lista1)):
    Producto = Producto + (Lista1[i]*Lista2[i])
print(Producto)
```

3.Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.
```python
# Inicializa un arreglo vacío para almacenar los números
arreglo_numeros = []
cantidad_arreglo = int(input("¿De cuantos numeros quiere el arreglo?:"))

primer_numero = int(input("Ingrese su primer numero para el arreglo:"))
arreglo_numeros.append(primer_numero)

# Utiliza un bucle for para pedir al usuario los números intermedios
for i in range(cantidad_arreglo - 2):
    numeros = int(input("Ingrese el siguiente numero: "))
    arreglo_numeros.append(numeros)

ultimo_numero = int(input("Ingrese el ultimo numero para el arreglo:"))
arreglo_numeros.append(ultimo_numero)


# Imprime el arreglo de números original
print("Su arreglo de numeros es:" + str(arreglo_numeros))


# Recorre el arreglo de números
for numero in arreglo_numeros:
    # Si el número es 0, lo agrega al final del arreglo y lo elimina de su posición actual
    if numero == 0:
        arreglo_numeros.append(numero)
        arreglo_numeros.remove(numero)
    # Si el número no es 0, continúa con la siguiente iteración del bucle
    else:
        if numero != 0:
            continue
````

4.Revisar que son los algoritmos de sorting, entender bubble-sort (enlace a implementación).
• Bubble-sort es un algoritmo de clasificación  el cual va  reemplazando iterativamente elementos  si están desordenados con el fin de ordenarlos de menor a mayor sin embargo existe un problema y es que este algoritmo no es adecuado para grandes conjuntos de datos porque su complejidad temporal se vuelve alta a medida que la lista incremente sus elementos ya que utilizaria mas condicionales.
