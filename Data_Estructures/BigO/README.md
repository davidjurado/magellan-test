# Big O Notation

En informática y programación, siempre estamos buscando soluciones "buenas". En muchos casos, la mejor solución es la que se realiza más rápido, que generalmente está relacionada con el uso de la menor cantidad de cálculos.

Para comparar significativamente el rendimiento algorítmico, podemos usar la notación Big O, a veces denominada "orden de crecimiento". En resumen, compara el comportamiento asintótico de los algoritmos; es decir, ¿cómo se escala su rendimiento en función del tamaño de entrada?

Informalmente, <a href="https://www.codecogs.com/eqnedit.php?latex=f(x)=O(g)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?f(x)=O(g)" title="f(x)=O(g)" /></a> si <a href="https://www.codecogs.com/eqnedit.php?latex=f" target="_blank"><img src="https://latex.codecogs.com/gif.latex?f" title="f" /></a> es "menor o más o menos del mismo tamaño" que <a href="https://www.codecogs.com/eqnedit.php?latex=g" target="_blank"><img src="https://latex.codecogs.com/gif.latex?g" title="g" /></a> cuando <a href="https://www.codecogs.com/eqnedit.php?latex=x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x" title="x" /></a> es muy grande.

Por ejemplo, considere dos algoritmos representados por <a href="https://www.codecogs.com/eqnedit.php?latex=f(x)=4x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?f(x)=4x" title="f(x)=4x" /></a> y <a href="https://www.codecogs.com/eqnedit.php?latex=g(x)=10x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?g(x)=10x" title="g(x)=10x" /></a>. Estos son "más o menos del mismo tamaño" cuando x es muy grande, así que <a href="https://www.codecogs.com/eqnedit.php?latex=4x=O(10x)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?4x=O(10x)" title="4x=O(10x)" /></a> y <a href="https://www.codecogs.com/eqnedit.php?latex=10x=O(4x)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?10x=O(4x)" title="10x=O(4x)" /></a>.

Por otro lado, al comparar <a href="https://www.codecogs.com/eqnedit.php?latex=4x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?4x" title="4x" /></a> y <a href="https://www.codecogs.com/eqnedit.php?latex=x^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x^2" title="x^2" /></a> se infiere que <a href="https://www.codecogs.com/eqnedit.php?latex=4x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?4x" title="4x" /></a> es menor que <a href="https://www.codecogs.com/eqnedit.php?latex=x^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x^2" title="x^2" /></a> cuando <a href="https://www.codecogs.com/eqnedit.php?latex=x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x" title="x" /></a> se hace muy grande, por lo que <a href="https://www.codecogs.com/eqnedit.php?latex=4x=O(x^2)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?4x=O(x^2)" title="4x=O(x^2)" /></a> pero <a href="https://www.codecogs.com/eqnedit.php?latex=x^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x^2" title="x^2" /></a> no es igual que <a href="https://www.codecogs.com/eqnedit.php?latex=O(4x)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(4x)" title="O(4x)" /></a>

Hablando formalmente <a href="https://www.codecogs.com/eqnedit.php?latex=f" target="_blank"><img src="https://latex.codecogs.com/gif.latex?f" title="f" /></a> y <a href="https://www.codecogs.com/eqnedit.php?latex=g" target="_blank"><img src="https://latex.codecogs.com/gif.latex?g" title="g" /></a> son funciones, donde <a href="https://www.codecogs.com/eqnedit.php?latex=f=O(g)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?f=O(g)" title="f=O(g)" /></a> si existe una constante <a href="https://www.codecogs.com/eqnedit.php?latex=C" target="_blank"><img src="https://latex.codecogs.com/gif.latex?C" title="C" /></a> tal que:

 <div align="center">
  <a href="https://www.codecogs.com/eqnedit.php?latex=|f(x)|&space;\leqslant&space;C.|g(x)|" target="_blank"><img src="https://latex.codecogs.com/gif.latex?|f(x)|&space;\leqslant&space;C.|g(x)|" title="|f(x)| \leqslant C.|g(x)|" /></a>
</div> 

Para una <a href="https://www.codecogs.com/eqnedit.php?latex=x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x" title="x" /></a> suficientemente grande.

El motivo de esta formulación es que no nos preocupan demasiado los factores constantes en el rendimiento algorítmico, sino la dependencia del tamaño de la entrada, especialmente cuando los conjuntos de datos pueden ser extraordinariamente grandes.

Cuando <a href="https://www.codecogs.com/eqnedit.php?latex=f=O(g)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?f=O(g)" title="f=O(g)" /></a>, estamos diciendo que cuando los tamaños de entrada se escalan para llegar a ser muy grandes, el rendimiento relativo de estos algoritmos es casi constante, por lo que se comportan "de manera similar".

Por ejemplo, si un algoritmo toma <a href="https://www.codecogs.com/eqnedit.php?latex=100Log_2(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?100Log_2(n)" title="100Log_2(n)" /></a> cálculos y otro toma <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a>, la constante <a href="https://www.codecogs.com/eqnedit.php?latex=100" target="_blank"><img src="https://latex.codecogs.com/gif.latex?100" title="100" /></a> se vuelve completamente irrelevanta para un <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> muy grande. Incluso para <a href="https://www.codecogs.com/eqnedit.php?latex=n=10000" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n=10000" title="n=10000" /></a>, el algoritmo <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> usa aproximadamente 10 veces más cálculos.

Además, cuando hablamos de la notación Big O, a menudo "soltamos" términos de menor grado y solo conservamos el más significativo. Hay que recordar que estamos viendo situaciones en las que los tamaños de las entradas se amplían para ser muy grandes, por eso es que se pueden descartar términos más bajos.

Por ejemplo, considere un algoritmo de dos partes donde la primera toma <a href="https://www.codecogs.com/eqnedit.php?latex=O(nLog_2(n))" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(nLog_2(n))" title="O(nLog_2(n))" /></a> y la segunda <a href="https://www.codecogs.com/eqnedit.php?latex=O(n^2)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n^2)" title="O(n^2)" /></a>. El tiempo de ejecución general para este algoritmo en la notación Big O sería <a href="https://www.codecogs.com/eqnedit.php?latex=O(n^2)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n^2)" title="O(n^2)" /></a>. Aunque técnicamente podemos escribir el tiempo de ejecución total como <a href="https://www.codecogs.com/eqnedit.php?latex=O(nLog_2(n)&space;&plus;&space;n^2)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(nLog_2(n)&space;&plus;&space;n^2)" title="O(nLog_2(n) + n^2)" /></a>, el termino <a href="https://www.codecogs.com/eqnedit.php?latex=n^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n^2" title="n^2" /></a> crece mucho más rápido que el termino <a href="https://www.codecogs.com/eqnedit.php?latex=nLog_2(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?nLog_2(n)" title="nLog_2(n)" /></a> cuando <a href="https://www.codecogs.com/eqnedit.php?latex=x" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x" title="x" /></a> se hace demasiado grande.

Comparar las eficiencias de diferentes soluciones para el mismo problema es una parte clave de la informática, y la notación Big O nos da una forma estandarizada de hacerlo.

Generalmente, el tiempo requerido por un algoritmo cae bajo tres tipos:

* Mejor caso: tiempo mínimo requerido para la ejecución del programa.

* Caso promedio - Tiempo promedio requerido para la ejecución del programa.

* Peor caso: tiempo máximo requerido para la ejecución del programa.

### Complejidades ordenadas de menor a mayor

* Tiempo constante: <a href="https://www.codecogs.com/eqnedit.php?latex=O(1)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(1)" title="O(1)" /></a>

* Tiempo logaritmico: <a href="https://www.codecogs.com/eqnedit.php?latex=O(Log(n))" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(Log(n))" title="O(Log(n))" /></a>

* Tiempo lineal: <a href="https://www.codecogs.com/eqnedit.php?latex=O(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n)" title="O(n)" /></a>

* Tiempo linearitmico: <a href="https://www.codecogs.com/eqnedit.php?latex=O(nLog(n))" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(nLog(n))" title="O(nLog(n))" /></a>

* Tiempo cuadrático: <a href="https://www.codecogs.com/eqnedit.php?latex=O(n^2)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n^2)" title="O(n^2)" /></a>

* Tiempo cúbico: <a href="https://www.codecogs.com/eqnedit.php?latex=O(n^3)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n^3)" title="O(n^3)" /></a>

* Tiempo exponencial: <a href="https://www.codecogs.com/eqnedit.php?latex=O(b^n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(b^n)" title="O(b^n)" /></a>, <a href="https://www.codecogs.com/eqnedit.php?latex=b>1" target="_blank"><img src="https://latex.codecogs.com/gif.latex?b>1" title="b>1" /></a>

* Tiempo factorial: <a href="https://www.codecogs.com/eqnedit.php?latex=O(n!)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n!)" title="O(n!)" /></a>

<p align="center">
  <img src="https://he-s3.s3.amazonaws.com/media/uploads/ece920b.png">
</p>



### Ejemplos

```java
public static void simpleFunction(int n){
	int a=9;
	int b=3;

	int sum=a+b+n;
	int product=a*b*n;
	int quotient=a*n/b;

	System.out.println(String.format(
		"The summ is: %s, product is: %s and quotient is: %s", sum,product,quotient));
}
```

Esta función es de tiempo constante, ya que cualquier que sea el valor de <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> demorará el mismo tiempo en ejecutarse, es de decir que es de orden <a href="https://www.codecogs.com/eqnedit.php?latex=O(1)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(1)" title="O(1)" /></a>.

<br>

```java
public static void singleForLoop(int n){
	for(int i=0; i<n; i++){
			System.out.println(String.format("Square of %s is: %s", i, Math.pow(i,2.0)));
	}
}
```

El ciclo imprime <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> veces el valor de <a href="https://www.codecogs.com/eqnedit.php?latex=i" target="_blank"><img src="https://latex.codecogs.com/gif.latex?i" title="i" /></a> e <a href="https://www.codecogs.com/eqnedit.php?latex=i^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?i^2" title="i^2" /></a>, por lo que la complejidad de este código es orden <a href="https://www.codecogs.com/eqnedit.php?latex=O(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n)" title="O(n)" /></a>.

<br>

```java
public static void nestedForLoop(int n){
	for(int i=0; i<n; i++){
		for(int j=0; j<n; j++){
		    System.out.println(String.format("Product of %s and %s is: %s", i, j, i*j));
		}
	}
}
```

En este caso se tienen dos ciclos anidados, por cada iteración del primer ciclo el segundo iterará <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> veces, entonces la complejidad de la función es <a href="https://www.codecogs.com/eqnedit.php?latex=O(n^2)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n^2)" title="O(n^2)" /></a>.

<br>

```java
public static void twoForLoops(int n){
	for(int i=0; i<n; i++){
		System.out.println("Printing: " + i);
	}
	for(int i=0; i<1000; i++){
		System.out.println("Printing: " + i);
	}
}
```
En este caso hay dos ciclos, pero el primero va de <a href="https://www.codecogs.com/eqnedit.php?latex=0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?0" title="0" /></a> a <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> y el segundo de <a href="https://www.codecogs.com/eqnedit.php?latex=0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?0" title="0" /></a> a <a href="https://www.codecogs.com/eqnedit.php?latex=1000" target="_blank"><img src="https://latex.codecogs.com/gif.latex?1000" title="1000" /></a>, la idea es asumir que <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> será muy grande, por lo que la complejidad sería <a href="https://www.codecogs.com/eqnedit.php?latex=O(n&plus;100)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n&plus;100)" title="O(n+100)" /></a>, pero la constante se ignora completamente ya que es insignificante ante <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> (que es muy grande), dando como resultado final que la complejidad es de orden <a href="https://www.codecogs.com/eqnedit.php?latex=O(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n)" title="O(n)" /></a>

<br>

```java
public static void twoForLoopsNAndM(int n, int m){
	for(int i=0; i<n; i++){
		for(int j=0; j<m; j++){
		    System.out.println("Printing: " + (i*j));
		}
	}
}
```

Existen dos ciclos anidados, pero en este caso se tienen dos entradas, haciendo que el primer ciclo itere en <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> y el segundo en <a href="https://www.codecogs.com/eqnedit.php?latex=m" target="_blank"><img src="https://latex.codecogs.com/gif.latex?m" title="m" /></a>, se asume que ambas entradas tienden a ser sumamente grandes dando como resultado una complejidad de orden <a href="https://www.codecogs.com/eqnedit.php?latex=O(n*m)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(n*m)" title="O(n*m)" /></a>.

<br>

```java
public static void doublingLoopVariable(int n){
	for(int i=1; i<n;){
		System.out.println("Value of i is: " + i);
		i=i*2;
	}
}
```

La variable del ciclo aumenta de una manera diferente, se está duplicando durante cada iteración, por lo que el ciclo se culminará mucho más rápido. Los resultados para cada ciclo serán:

1) <a href="https://www.codecogs.com/eqnedit.php?latex=i*2=1*2=2&space;\rightarrow&space;2^1" target="_blank"><img src="https://latex.codecogs.com/gif.latex?i*2=1*2=2&space;\rightarrow&space;2^1" title="i*2=1*2=2 \rightarrow 2^1" /></a> 	

2) <a href="https://www.codecogs.com/eqnedit.php?latex=i*2=2*2=4&space;\rightarrow&space;2^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?i*2=2*2=4&space;\rightarrow&space;2^2" title="i*2=2*2=4 \rightarrow 2^2" /></a>

3) <a href="https://www.codecogs.com/eqnedit.php?latex=i*2=4*2=8&space;\rightarrow&space;2^3" target="_blank"><img src="https://latex.codecogs.com/gif.latex?i*2=4*2=8&space;\rightarrow&space;2^3" title="i*2=4*2=8 \rightarrow 2^3" /></a>

.
.
.

k+1. <a href="https://www.codecogs.com/eqnedit.php?latex=i*2=2^(k-1)*2&space;\rightarrow&space;2^k" target="_blank"><img src="https://latex.codecogs.com/gif.latex?i*2=2^(k-1)*2&space;\rightarrow&space;2^k" title="i*2=2^(k-1)*2 \rightarrow 2^k" /></a>

Existe un <a href="https://www.codecogs.com/eqnedit.php?latex=k" target="_blank"><img src="https://latex.codecogs.com/gif.latex?k" title="k" /></a> tal que <a href="https://www.codecogs.com/eqnedit.php?latex=2^k=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?2^k=n" title="2^k=n" /></a>, en este punto es donde termina  el ciclo. El número de veces que se ejecuta el ciclo es <a href="https://www.codecogs.com/eqnedit.php?latex=k" target="_blank"><img src="https://latex.codecogs.com/gif.latex?k" title="k" /></a>.

Despejando <a href="https://www.codecogs.com/eqnedit.php?latex=k" target="_blank"><img src="https://latex.codecogs.com/gif.latex?k" title="k" /></a> tenemos que es igual a <a href="https://www.codecogs.com/eqnedit.php?latex=k=&space;log_2⁡(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?k=&space;log_2⁡(n)" title="k= log_2⁡(n)" /></a>. Es este resultado la verdadera complejidad de este algoritmo, es decir que es <a href="https://www.codecogs.com/eqnedit.php?latex=O(k)&space;\rightarrow&space;O(Log_2(n))" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(k)&space;\rightarrow&space;O(Log_2(n))" title="O(k) \rightarrow O(Log_2(n))" /></a>.

<br>

```java
public static void halvingLoopVariable(int n){
	for(int i=n; i>0;){
		System.out.println("Value of i is: " + i);
		i=i/2;
	}
}
```

Este caso es similar al anterior, solo que acá el ciclo va de <a href="https://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n" title="n" /></a> a <a href="https://www.codecogs.com/eqnedit.php?latex=0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?0" title="0" /></a> y la variable se está diviendo en la mitad en cada iteración haciendo que el ciclo acabe más rápido, en este caso el orden es de <a href="https://www.codecogs.com/eqnedit.php?latex=O(Log(n))" target="_blank"><img src="https://latex.codecogs.com/gif.latex?O(Log(n))" title="O(Log(n))" /></a>.