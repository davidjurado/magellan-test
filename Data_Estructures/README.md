# Estructuras de datos, algoritmos y complejidad

## Estructuras de datos

### Qué es una estructua de datos?
<div class="box">
  "Es una forma particular de almacenar datos organizados en un computador para que se pueda usar de manera eficiente."
</div>

- Ejemplos de estructuras de datos:
  - Estructura `Persona` (Nombre + Apellido + Edad)
  - Array de enteros – `int[]`
  - Lista de strings – `List<string>`
  - Fila de personas – `Queue<Person>`

## Tipos de datos

### Tipos primitivos

* Boolean, true or false.
* Character
* Números de coma flotante, valores de número racional de precisión limitados.
* Fixed-point numbers
* Integer, integral or fixed-precision values.
* Reference (also called a pointer or handle), a small value referring to another object's address in memory, possibly a much larger one.
* Enumerated type, a small set of uniquely named values.

Tipos compuestos o tipo no primitivo

* Array
* Record (also called tuple or structure)
* String, a sequence of characters.
* Union
* Tagged union (also called variant, variant record, discriminated union, or disjoint union)

Tipos de datos abstractos

* Container
* List
* Associative array
* Multimap
* Heap
* Set
* Multiset (bag)
* Stack
* Queue
* Double-ended queue
* Priority queue
* Tree
* Graph

### Estructuras de datos lineales

Se dice que una estructura de datos es lineal si sus elementos forman una secuencia.

Matrices

* Array
* Bit array
* Bit field
* Bitboard
* Bitmap
* Circular buffer
* Control table
* Image
* Dope vector
* Dynamic array
* Gap buffer
* Hashed array tree
* Heightmap
* Lookup table
* Matrix
* Parallel array
* Sorted array
* Sparse matrix
* Iliffe vector
* Variable-length array

Listas

* Doubly linked list
* Array list
* Linked list
* Self-organizing list
* Skip list
* Unrolled linked list
* VList
* Conc-tree list
* Xor linked list
* Zipper
* Doubly connected edge list also known as half-edge
* Difference list
* Free list

### Árboles

Árboles binarios

* AA tree
* AVL tree
* Binary search tree
* Binary tree
* Cartesian tree
* Left-child right-sibling binary tree
* Order statistic tree
* Pagoda
* Randomized binary search tree
* Red–black tree
* Rope
* Scapegoat tree
* Self-balancing binary search tree
* Splay tree
* T-tree
* Tango tree
* Threaded binary tree
* Top tree
* Treap
* WAVL tree
* Weight-balanced tree

B-trees

* B-tree
* B+ tree
* B*-tree
* B sharp tree
* Dancing tree
* 2-3 tree
* 2-3-4 tree
* Queap
* Fusion tree
* Bx-tree
* AList

Heaps

* Heap
* Binary heap
* B-heap
* Weak heap
* Binomial heap
* Fibonacci heap
* AF-heap
* Leonardo Heap
* 2-3 heap
* Soft heap
* Pairing heap
* Leftist heap
* Treap
* Beap
* Skew heap
* Ternary heap
* D-ary heap
* Brodal queue

Tries

En estas estructuras de datos, cada nodo de árbol compara un fragmento de valores de clave.

* Trie
* Radix tree
* Suffix tree
* Suffix array
* Compressed suffix array
* FM-index
* Generalised suffix tree
* B-trie
* Judy array
* X-fast trie
* Y-fast trie
* Merkle tree
* Ctrie

Árboles multiway

* Ternary tree
* K-ary tree
* And–or tree
* (a,b)-tree
* Link/cut tree
* SPQR-tree
* Spaghetti stack
* Disjoint-set data structure
* Fusion tree
* Enfilade
* Exponential tree
* Fenwick tree
* Van Emde Boas tree
* Rose tree

Árboles de partición de espacio

Estas son estructuras de datos usadas para la partición del espacio o la partición del espacio binario.

* Segment tree
* Interval tree
* Range tree
* Bin
* K-d tree
* Implicit k-d tree
* Min/max k-d tree
* Relaxed k-d tree
* Adaptive k-d tree
* Quadtree
* Octree
* Linear octree
* Z-order
* UB-tree
* R-tree
* R+ tree
* R* tree
* Hilbert R-tree
* X-tree
* Metric tree
* Cover tree
* M-tree
* VP-tree
* BK-tree
* Bounding interval hierarchy
* Bounding volume hierarchy
* BSP tree
* Rapidly exploring random tree

Árboles específicos de la aplicación

* Abstract syntax tree
* Parse tree
* Decision tree
* Alternating decision tree
* Minimax tree
* Expectiminimax tree
* Finger tree
* Expression tree
* Log-structured merge-tree
* Lexicographic Search Tree

Hashes

* Bloom filter
* Count-Min sketch
* Distributed hash table
* Double hashing
* Dynamic perfect hash table
* Hash array mapped trie
* Hash list
* Hash table
* Hash tree
* Hash trie
* Koorde
* Prefix hash tree
* Rolling hash
* MinHash
* Quotient filter
* Ctrie

Graphs

* Graph
* Adjacency list
* Adjacency matrix
* Graph-structured stack
* Scene graph
* Binary decision diagram
* Zero-suppressed decision diagram
* And-inverter graph
* Directed graph
* Directed acyclic graph
* Propositional directed acyclic graph
* Multigraph
* Hypergraph

Otros

* Lightmap
* Winged edge
* Quad-edge
* Routing table
* Symbol table

## Complejidad del tiempo

En informática, la complejidad del tiempo es la complejidad computacional que describe la cantidad de tiempo que lleva correr un algoritmo. La complejidad del tiempo se suele calcular contando el número de operaciones elementales realizadas por el algoritmo, suponiendo que cada operación elemental lleva una cantidad de tiempo fija. Por lo tanto, se considera que la cantidad de tiempo empleado y el número de operaciones elementales realizadas por el algoritmo difieren en un factor constante como máximo.

Dado que el tiempo de ejecución de un algoritmo puede variar entre diferentes tipos de entrada, se suele considerar la complejidad de tiempo del peor de los casos, que es la cantidad de tiempo máxima requerida para las entradas de un tamaño determinado. Menos común, y generalmente especificado explícitamente, es la complejidad del caso promedio, que es el promedio del tiempo empleado en las entradas de un tamaño dado (esto tiene sentido porque solo hay un número finito de entradas posibles de un tamaño dado). En ambos casos, la complejidad del tiempo generalmente se expresa como una función del tamaño de la entrada. Dado que esta función es generalmente difícil de calcular exactamente, y el tiempo de ejecución para las entradas pequeñas generalmente no es consecuente, se suele enfocar sobre el comportamiento de la complejidad cuando aumenta el tamaño de entrada, es decir, el comportamiento asintótico de la complejidad. Por lo tanto, la complejidad del tiempo se expresa habitualmente usando la notación (Big O), por lo general O (n), O(nLogn(n)), O(n^2), etc. donde n es el tamaño de entrada en unidades de bits necesarios para representar la entrada.

<p align="center">
    <img  src="https://cooervo.github.io/Algorithms-DataStructures-BigONotation/images/graphs/comparison.svg" style="width: 40%; height: 40%">
</p>

# Operaciones comunes de estructura de datos

Below are the Big O performance of common functions of different Java Collections.


List                 | Add  | Remove | Get  | Contains | Next | Data Structure
---------------------|------|--------|------|----------|------|---------------
ArrayList            | O(1) |  O(n)  | O(1) |   O(n)   | O(1) | Array
LinkedList           | O(1) |  O(1)  | O(n) |   O(n)   | O(1) | Linked List
CopyOnWriteArrayList | O(n) |  O(n)  | O(1) |   O(n)   | O(1) | Array

<br>
<br>

Set                   |    Add   |  Remove  | Contains |   Next   | Size | Data Structure
----------------------|----------|----------|----------|----------|------|-------------------------
HashSet               | O(1)     | O(1)     | O(1)     | O(h/n)   | O(1) | Hash Table
LinkedHashSet         | O(1)     | O(1)     | O(1)     | O(1)     | O(1) | Hash Table + Linked List
EnumSet               | O(1)     | O(1)     | O(1)     | O(1)     | O(1) | Bit Vector
TreeSet               | O(log n) | O(log n) | O(log n) | O(log n) | O(1) | Red-black tree
CopyOnWriteArraySet   | O(n)     | O(n)     | O(n)     | O(1)     | O(1) | Array
ConcurrentSkipListSet | O(log n) | O(log n) | O(log n) | O(1)     | O(n) | Skip List

<br>
<br>

Queue                   |  Offer   | Peak |   Poll   | Remove | Size | Data Structure
------------------------|----------|------|----------|--------|------|---------------
PriorityQueue           | O(log n) | O(1) | O(log n) |  O(n)  | O(1) | Priority Heap
LinkedList              | O(1)     | O(1) | O(1)     |  O(1)  | O(1) | Array
ArrayDequeue            | O(1)     | O(1) | O(1)     |  O(n)  | O(1) | Linked List
ConcurrentLinkedQueue   | O(1)     | O(1) | O(1)     |  O(n)  | O(n) | Linked List
ArrayBlockingQueue      | O(1)     | O(1) | O(1)     |  O(n)  | O(1) | Array
PriorirityBlockingQueue | O(log n) | O(1) | O(log n) |  O(n)  | O(1) | Priority Heap
SynchronousQueue        | O(1)     | O(1) | O(1)     |  O(n)  | O(1) | None!
DelayQueue              | O(log n) | O(1) | O(log n) |  O(n)  | O(1) | Priority Heap
LinkedBlockingQueue     | O(1)     | O(1) | O(1)     |  O(n)  | O(1) | Linked List

<br>
<br>

Map                   |   Get    | ContainsKey |   Next   | Data Structure
----------------------|----------|-------------|----------|-------------------------
HashMap               | O(1)     |   O(1)      | O(h / n) | Hash Table
LinkedHashMap         | O(1)     |   O(1)      | O(1)     | Hash Table + Linked List
IdentityHashMap       | O(1)     |   O(1)      | O(h / n) | Array
WeakHashMap           | O(1)     |   O(1)      | O(h / n) | Hash Table
EnumMap               | O(1)     |   O(1)      | O(1)     | Array
TreeMap               | O(log n) |   O(log n)  | O(log n) | Red-black tree
ConcurrentHashMap     | O(1)     |   O(1)      | O(h / n) | Hash Tables
ConcurrentSkipListMap | O(log n) | O(log n) | O(1) | Skip List

<br>
<br>


## Complejidad algorítmica


<table style="undefined;table-layout: fixed; width: 810px">
<colgroup>
<col style="width: 177px">
<col style="width: 117px">
<col style="width: 176px">
<col style="width: 156px">
<col style="width: 184px">
</colgroup>
  <tr>
    <th>Algoritmo</th>
    <th colspan="3">Complejidad del tiempo</th>
    <th><br>Complejidad espacial</th>
  </tr>
  <tr>
    <td></td>
    <td>Mejor</td>
    <td>Promedio</td>
    <td>Peor</td>
    <td>Peor</td>
  </tr>
  <tr>
    <td>Quicksort</td>
    <td>O(nLog(n))</td>
    <td>O(nLog(n))</td>
    <td>O(n^2)</td>
    <td>O(Log(n))</td>
  </tr>
  <tr>
    <td>Mergesort</td>
    <td>O(nLog(n))</td>
    <td>O(nLog(n))</td>
    <td>O(nLog(n))</td>
    <td>O(n)</td>
  </tr>
  <tr>
    <td>Timsort</td>
    <td><br>O(n)</td>
    <td>O(nLog(n))</td>
    <td>O(nLog(n))</td>
    <td>O(n)</td>
  </tr>
  <tr>
    <td>Heapsort</td>
    <td>O(nLog(n))</td>
    <td>O(nLog(n))</td>
    <td>O(nLog(n))</td>
    <td>O(1)</td>
  </tr>
  <tr>
    <td><br>Bubble Sort</td>
    <td>O(n)</td>
    <td>O(n^2)</td>
    <td>O(n^2)</td>
    <td>O(1)</td>
  </tr>
  <tr>
    <td><br>Insertion Sort <br></td>
    <td>O(n)</td>
    <td>O(n^2)</td>
    <td>O(n^2)</td>
    <td>O(1)</td>
  </tr>
  <tr>
    <td>Selection Sort<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td>O(n^2)</td>
    <td>O(n^2)</td>
    <td>O(n^2)</td>
    <td>O(1)</td>
  </tr>
  <tr>
    <td>Tree sort<br></td>
    <td>O(nLog(n))</td>
    <td>O(nLog(n))</td>
    <td>O(n^2)</td>
    <td>O(n)</td>
  </tr>
  <tr>
    <td><br>Shell Sort</td>
    <td>O(nLog(n))</td>
    <td>O(n(Log(n))n^2)</td>
    <td>O(n(Log(n))n^2)</td>
    <td>O(1)</td>
  </tr>
  <tr>
    <td><br>Bucket sort</td>
    <td>O(n+k)</td>
    <td>O(n+k)</td>
    <td>O(n^2)</td>
    <td>O(n)</td>
  </tr>
  <tr>
    <td>Radix sort<br></td>
    <td>O(nk)</td>
    <td>O(nk)</td>
    <td>O(nk)</td>
    <td>O(n+k)</td>
  </tr>
  <tr>
    <td>Counting Sort<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td>
    <td>O(n+k)</td>
    <td>O(n+k)</td>
    <td>O(n+k)</td>
    <td><br>O(k)</td>
  </tr>
  <tr>
    <td>Cubesort</td>
    <td>O(n)</td>
    <td>O(nLog(n))</td>
    <td>O(nLog(n))</td>
    <td>O(n)</td>
  </tr>
</table>