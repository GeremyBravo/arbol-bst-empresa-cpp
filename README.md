Árbol Binario de Búsqueda
Un Árbol Binario de Búsqueda (BST) es una estructura de datos jerárquica donde cada nodo tiene como máximo dos hijos. La propiedad fundamental es que todos los nodos del subárbol izquierdo tienen valores menores al nodo padre, y todos los del subárbol derecho tienen valores mayores.
Conceptos Clave
•	Raiz: nodo superior del árbol, sin padre.
•	Nodo interno: nodo que tiene al menos un hijo.
•	Hoja: nodo sin hijos.
•	Altura: numero de niveles desde la raiz hasta la hoja mas lejana.
•	Nivel: profundidad de un nodo dentro del arbol.
Recorridos
•	Inorden (Izquierda - Raiz - Derecha): produce los elementos ordenados de menor a mayor.
•	Preorden (Raiz - Izquierda - Derecha): util para copiar o serializar el arbol.
•	Postorden (Izquierda - Derecha - Raiz): util para liberar memoria o evaluar expresiones.
Descripción del Programa
El programa implementa un menú interactivo en consola con las siguientes funcionalidades:
•	Insertar empleado (código, nombre, cargo)
•	Buscar empleado por código
•	Mostrar la raíz del árbol
•	Recorrido inorden
•	Recorrido preorden
•	Recorrido postorden
•	Calcular y mostrar la altura del arbol
•	Identificar y mostrar los nodos hoja
Estructura del Código
Struct Empleado
Almacena los datos de cada empleado: código (int), nombre (string) y cargo (string).
Struct Nodo
Representa cada nodo del árbol. Contiene un objeto Empleado y punteros al hijo izquierdo y derecho. El constructor inicializa ambos punteros en nullptr.
Clase ArbolBST
Contiene el puntero a la raíz y los métodos privados recursivos para insertar, buscar, recorrer, calcular altura y mostrar hojas. Los métodos públicos son la interfaz para el main.


Capturas
1.	Menú principal
==== MENU ARBOL BST EMPRESARIAL ====

Insertar empleado

Buscar empleado

Mostrar raíz

Recorrido inorden

Recorrido preorden

Recorrido postorden

Mostrar altura

Mostrar hojas

Salir

2.	Inserción de empleados
Seleccione una opción: 1
Codigo: 50
Nombre: Empresa UTA
Cargo: Raíz

3.	Búsqueda
Seleccione una opción: 2
Ingrese código a buscar: 70

Empleado encontrado:
Codigo: 70 | Nombre: Gerente Finanzas | Cargo: Nodo interno

4.	Recorridos
•	Mostrar recorrido inorden.
Recorrido Inorden:
Codigo: 20 | Nombre: Emp | Cargo: Hoja
Codigo: 30 | Nombre: Gerente Ventas | Cargo: Nodo interno
Codigo: 40 | Nombre: Emp 2 | Cargo: Hoja
Codigo: 50 | Nombre: Empresa UTA | Cargo: Raíz
Codigo: 60 | Nombre: Emp 3 | Cargo: Hoja
Codigo: 70 | Nombre: Gerente Finanzas | Cargo: Nodo interno
Codigo: 80 | Nombre: Emp 4 | Cargo: Hoja

•	Mostrar recorrido preorden.
Recorrido Preorden:
Codigo: 50 | Nombre: Empresa UTA | Cargo: Raíz
Codigo: 30 | Nombre: Gerente Ventas | Cargo: Nodo interno
Codigo: 20 | Nombre: Emp | Cargo: Hoja
Codigo: 40 | Nombre: Emp 2 | Cargo: Hoja
Codigo: 70 | Nombre: Gerente Finanzas | Cargo: Nodo interno
Codigo: 60 | Nombre: Emp 3 | Cargo: Hoja
Codigo: 80 | Nombre: Emp 4 | Cargo: Hoja

•	Mostrar recorrido postorden.
Recorrido Postorden:
Codigo: 20 | Nombre: Emp | Cargo: Hoja
Codigo: 40 | Nombre: Emp 2 | Cargo: Hoja
Codigo: 30 | Nombre: Gerente Ventas | Cargo: Nodo interno
Codigo: 60 | Nombre: Emp 3 | Cargo: Hoja
Codigo: 80 | Nombre: Emp 4 | Cargo: Hoja
Codigo: 70 | Nombre: Gerente Finanzas | Cargo: Nodo interno
Codigo: 50 | Nombre: Empresa UTA | Cargo: Raíz
 
5.	Altura y hoja.
Mostrar altura del árbol
Seleccione una opcion: 7

Altura del arbol: 3

Mostrar nodos hoja
Seleccione una opcion: 8

Nodos hoja:
Codigo: 20 | Nombre: Emp | Cargo: Hoja
Codigo: 40 | Nombre: Emp 2 | Cargo: Hoja
Codigo: 60 | Nombre: Emp 3 | Cargo: Hoja
Codigo: 80 | Nombre: Emp 4 | Cargo: Hoja

