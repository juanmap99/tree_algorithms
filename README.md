# Manual de usuario
Esta herramienta permite entender de manera visual, textual y experimental la manera que funcionan los árboles cubiertos.

Los árboles desarrollados son:
 
 * **Árboles**
	- BST (Binary Search Tree)
	- AVL Tree (Adelson-Velsky and Landis)
	- RBT (Red Black Tree)
	 - Max Heap
	 - Min Heap
	 - Treap

## **Configuración**
Los parámetros que se le permite al usuario ajustar son los siguientes:
- **Altura:** Este parámetro define la altura del árbol generado mediante valores aleatorios. A excepción del Treap, el usuario puede elegir la altura deseada dentro de un rango de 0 a 4 (inclusive). Es importante mencionar que el Treap se encuentra limitado debido a que, dada su naturaleza, podría exceder este límite si se generará aleatoriamente. Los detalles sobre esta restricción se explicarán en una sección posterior.
- **Velocidad:** Este parámetro determina el tiempo de retraso entre cada paso del algoritmo durante la ejecución automática. A medida que se incrementa la velocidad, disminuye el retraso entre cada paso del algoritmo. Se cuentan con cinco velocidades, en donde el retraso asociado a cada una de ellas es el siguiente:
	- Velocidad 1: 500 ms
	- Velocidad 2: 250 ms
	- Velocidad 3: 100 ms
	- Velocidad 4: 60 ms
	- Velocidad 5: 30 ms
- **Método:** Este parámetro define el método a ejecutar. Los métodos predefinidos son:
	- Add
	- Search
	- Delete. Es relevante destacar que, en el caso de las Max Heap, el método Delete es reemplazado por Pop Max, mientras que en las Min Heap es reemplazado por Pop Min.
	- FindMax
	- FindMin
	- InOrder
	- PreOrder
	- PostOrder
- **Elemento:** Este valor numérico determina el valor del nodo al ejecutar los métodos Add, Search o Delete. Cabe señalar que, para los métodos FindMax, FindMin, PopMax o PopMin, el campo se encuentra deshabilitado en la herramienta. Además, por cuestiones visuales relacionadas con el tamaño de la fuente y el diámetro del círculo que representa a cada nodo, el valor ingresado debe estar en el rango de -99 a 999.	

## Restricciones
La restricción más relevante que se ha aplicado se relaciona con la altura máxima de cuatro niveles permitida para el crecimiento del árbol, exceptuando el Red Black Tree en el cual los hijos NULL se representan gráficamente y el límite se establece en tres niveles.

La decisión de imponer un límite de altura en cuatro radica en una consideración sobre la relación entre la cantidad de nodos en una capa y la siguiente. En este contexto, la cantidad de nodos en una capa determinada es el doble de la cantidad en la capa previa. Permitir árboles de una altura mayor, específicamente de cinco capas, implicaría graficar 32 nodos en la última capa.

Tomando dicho contexto en referencia, se consideró que permitir árboles con más de cuatro capas podría afectar la legibilidad y estructura característica del árbol en pantalla. Dado que esto podría impactar negativamente en la experiencia del usuario y excluir ciertos dispositivos con pantallas más pequeñas, se optó por limitar la altura a cuatro capas.

A pesar de esta restricción, una altura de cuatro niveles es más que adecuada para visualizar y comprender todas las funcionalidades implementadas.
## Estructura del código
El usuario puede activar el código correspondiente presionando el botón "Código" ubicado en la sección inferior de la configuración.

Al pulsar este botón, se abre una ventana modal en el centro de la pantalla, de manera similar a la explicación, que contiene el código desarrollado en Python para el algoritmo en cuestión.

Dentro de esta modal, el usuario cuenta con las siguientes opciones:
- **Copiar el código:** Se proporciona un botón en la esquina superior derecha de la ventana modal, que permite al usuario copiar fácilmente el código presentado.
- **Cambiar el tema visual:** Se brinda la posibilidad de alternar entre dos temas visuales:  “Light Theme” y “Dark Theme”, ajustándose así a las preferencias visuales del usuario.
