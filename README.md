# Manual de usuario
Esta herramienta permite comprender de manera visual, textual y práctica el funcionamiento de diversos tipos de árboles.

## Árboles Implementados
La herramienta incluye los siguientes tipos de árboles:

- BST (Binary Search Tree)
- AVL Tree (Adelson-Velsky and Landis)
- RBT (Red Black Tree)
 - Max Heap
 - Min Heap
 - Treap

## Configuración
La herramienta permite a los usuarios personalizar varios parámetros para ajustar el comportamiento y las operaciones de los árboles:

### 1. Altura
Define la altura máxima del árbol generado aleatoriamente. La altura puede configurarse entre 0 y 4 (inclusive), excepto en el caso del Treap, que tiene un límite diferente debido a su naturaleza. El Treap puede exceder este rango si se genera aleatoriamente; esta limitación se detalla en la sección de Restricciones.

### 2. Velocidad
Controla el tiempo de retraso entre los pasos del algoritmo en las ejecuciones automáticas. A mayor velocidad, menor retraso. Las opciones disponibles son:

- **Velocidad 1:** 500 ms
- **Velocidad 2:** 250 ms
- **Velocidad 3:** 100 ms
- **Velocidad 4:** 60 ms
- **Velocidad 5:** 30 ms

### 3. Método
Permite seleccionar la operación que se desea realizar en el árbol. Los métodos disponibles incluyen:

- Add (Agregar)
- Search (Buscar)
- Delete (Eliminar): En el caso de Max Heap y Min Heap, este método se reemplaza por Pop Max y Pop Min, respectivamente.
- FindMax (Buscar Máximo)
- FindMin (Buscar Mínimo)
- InOrder (Recorrido InOrder)
- PreOrder (Recorrido PreOrder)
- PostOrder (Recorrido PostOrder)

### 4. Elemento
Especifica el valor numérico del nodo a operar para los métodos Add, Search o Delete. Este campo está deshabilitado para los métodos FindMax, FindMin, Pop Max y Pop Min.

Por motivos visuales, el valor ingresado debe estar en el rango de -99 a 999. Esto asegura una correcta representación gráfica en pantalla, evitando problemas con el tamaño de los nodos y la legibilidad.

## Restricciones
### Altura Máxima del Árbol
La altura máxima permitida para los árboles es de cuatro niveles, con una excepción en el caso del Red Black Tree, donde los nodos hijos NULL se representan gráficamente y el límite se establece en tres niveles.

#### Razones del Límite
El límite de altura está diseñado para mantener la claridad visual y funcionalidad de la herramienta. Dado que la cantidad de nodos en una capa se duplica con respecto a la capa anterior, un árbol con cinco niveles tendría 32 nodos en la última capa, lo que podría afectar negativamente la experiencia del usuario al dificultar la visualización en dispositivos con pantallas más pequeñas.

Con este límite de cuatro niveles, la herramienta asegura una experiencia fluida y adecuada para estudiar todas las funcionalidades implementadas.

## Visualización del Código
La herramienta permite acceder al código fuente correspondiente al árbol seleccionado. Para ello, el usuario debe presionar el botón "Código", ubicado en la parte inferior de la sección de configuración.

### Funciones Disponibles en la Vista de Código

- **Visualización del Código:** Se muestra el código Python correspondiente al árbol y método seleccionados.
- **Copiar Código:** Un botón en la esquina superior derecha permite copiar el código al portapapeles.
- **Cambio de Tema:** El usuario puede alternar entre los modos "Light Theme" y "Dark Theme" para ajustar la apariencia de la interfaz según sus preferencias.
