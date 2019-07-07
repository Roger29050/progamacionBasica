# progamacionBasica

# Python

Es un lenguaje de programación interpretado de tipado dinámico cuya filosofía hace hincapié en una sintaxis que favorezca un código legible. Se trata de un lenguaje de programación multiparadigma y disponible en varias plataformas.

Dicho de otro modo, Python es:
•	Interpretado: Se ejecuta sin necesidad de ser procesado por el compilador y se detectan los errores en tiempo de ejecución.
•	Multiparadigma: Soporta programación funcional, programación imperativa y programación orientada a objetos.
•	Tipado dinámico: Las variables se comprueban en tiempo de ejecución.
•	Multiplataforma: disponible para plataformas de Windows, Linux o MAC.
•	Gratuito: No dispone de licencia para programar.
 
Al hacer uso de una sintaxis legible, la curva de aprendizaje es muy rápida, siendo de este modo, uno de los mejores lenguajes para iniciarse en la programación en modo texto. Por ejemplo, si comparamos un código escrito en lenguaje de programación por bloques como Blockly y el mismo código lo escribimos utilizando Python, vemos las similitudes en las instrucciones.

Python contiene una gran cantidad de librerías, tipos de datos y funciones incorporadas en el propio lenguaje, que ayudan a realizar muchas tareas comunes sin necesidad de tener que programarlas desde cero. Pero lo que realmente le hace brillante utilizándolo en una Raspberry Pi, es por la capacidad de poder utilizar los pines GPIO para conectar el mundo físico con el mundo digital.

## Como ejecutar el código

Se debe de escribir el código en un editor de texto como bloc de notas o algún otro y posteriormente guardarlo con el nombre que se desee (finaliza el nombre con '.py') y al guardarlo en la opción tipo selecciona 'todos los documentos'

Para ejecutar el código se necesita abrir la central de python que se llama anaconda prompt, después de eso se usara el comando ‘dir’ para desplegar las carpetas del equipo y cd para leer una en específico 'cd documentos' y cuando se consiga llegar a la carpeta en la que esta guardado mi documento se coloca python y el nombre del documento, al dar enter se correrá el código.


## 1.- El programa 'hola mundo'

El Hola Mundo se caracteriza por su sencillez, especialmente cuando se ejecuta en una interfaz de línea de comandos. En interfaces gráficas la creación de este programa requiere de más pasos.
El programa Hola Mundo también puede ser útil como prueba de configuración para asegurar que el compilador, el entorno de desarrollo y el entorno de ejecución estén instalados correctamente y funcionando.
Se escribiría de la siguiente manera:

print('Hola mundo')  ->Hola mundo

## 2.-Números y operaciones aritmeticas:

### Enteros y decimales

Python distingue entre números enteros y decimales. Al escribir un número decimal, el separador entre la parte entera y la parte decimal es un punto.

3->3

4.5->4.5

Si se escribe un número con parte decimal 0, Python considera el número como número decimal.

3.0->3.0

Se puede escribir un número decimal sin parte entera, pero lo habitual es escribir siempre la parte entera:

.3->0.3

### Las cuatro operaciones básicas

Las cuatro operaciones aritméticas básicas son la suma (+), la resta (-), la multiplicación (*) y la división (/).

Al hacer operaciones en las que intervienen números enteros y decimales, el resultado es siempre decimal. En el caso de que el resultado no tenga parte decimal, Python escribe 0 como parte decimal para indicar que el resultado es un número decimal:

4.5 * 3->13.5

4.5 * 2->9.0

Al sumar, restar o multiplicar números enteros, el resultado es entero.

1 + 2->3

3 - 4->-1
5 * 6->30

Al dividir números enteros, el resultado es siempre decimal, aunque sea un número entero. Cuando Python escribe un número decimal, lo escribe siempre con parte decimal, aunque sea nula.

9 / 2->4.5

9 / 3->3.0

Cuando en una fórmula aparecen varias operaciones, Python las efectúa aplicando las reglas usuales de prioridad de las operaciones (primero multiplicaciones y divisiones, después sumas y restas).

1 + 2 * 3->7

10 - 4 * 2->2

En caso de querer que las operaciones se realicen en otro orden, se deben utilizar paréntesis.

(5 + 8) / (7 - 2)->2.6

Cociente de una división

El cociente de una división se calcula en Python con el operador //. El resultado es siempre un número entero, pero será de tipo entero o decimal dependiendo del tipo de los números empleados (en caso de ser decimal, la parte decimal es siempre cero). Por ejemplo:

10 // 3->3

10 // 4->2

20.0 // 7->2.0

20 // 6.0->3.0

### Potencias y raíces

Las potencias se calculan con el operador **, teniendo en cuenta que x ** y = xy.

Las potencias tienen prioridad sobre las multiplicaciones y divisiones.

Utilizando exponentes negativos o decimales se pueden calcular potencias inversas o raíces n-ésimas.

 
2 ** 3->8

10 ** -4->0.0001           # Recuerde que a-b= 1/ab

### La función integrada round()

Para redondear un número (por ejemplo, cuando se muestra al usuario el resultado final de un cálculo), se puede utilizar la función integrada round(). La función integrada round() admite uno o dos argumentos numéricos.

Si sólo hay un argumento, la función devuelve el argumento redondeado al entero más próximo:

round(4.35)->4

round(4.62)->5

Si se escriben dos argumentos, siendo el segundo un número entero, la función integrada round() devuelve el primer argumento redondeado en la posición indicada por el segundo argumento.

Si el segundo argumento es positivo, el primer argumento se redondea con el número de decimales indicado:

round(4.3527, 2)->4.35

## Variables en Programación

En Programación también existe el concepto de "variable", parecido pero no idéntico al concepto matemático.

Las variables
En Programación, las variables están asociadas a variables concretos. Además, cada lenguaje de programación tiene su forma de implementar el concepto de variable, por lo que lo que se explica a continuación es válido para muchos lenguajes de programación, aunque otros lenguajes de programación permiten otras posibilidades.

En muchos lenguajes de programación, una variable se puede entender como una especie de caja en la que se puede guardar un valor (por ejemplo, un valor numérico). Esa caja suele corresponder a una posición de memoria en la memoria del ordenador.
Las variables se representan también mediante letras o palabras completas: x, y, a, b, nombre, apellidos, edad, etc.
Cuando en esos lenguajes de programación escribimos la instrucción ...
a = 2

Entrada por teclado: la función input()
Índice de Python  Principio de la página

## Entrada por teclado La función input()

### Variables en input()

En Informática, la "entrada" de un programa son los datos que llegan al programa desde el exterior. Actualmente, el origen más habitual es el teclado.

Subrutinas y bibliotecas en Programación
A veces, en un determinado programa es necesario efectuar una misma tarea en distintos puntos del programa y, a menudo, en diferentes programas es necesario efectuar una misma tarea. Para evitar tener que volver a escribir una y otra vez las mismas instrucciones, casi todos los lenguajes de programación permiten agrupar porciones de programa y reutilizarlos en un mismo programa o en diferentes programas.

Estas agrupaciones de código fueron inventadas en 1951 por Maurice Wilkes, matemático y físico británico que construyó en 1949 el EDSAC, el primer ordenador que almacenaba los programas en la propia circuitería del ordenador. Por sus contribuciones a la informática, Wilkes recibió en 1967 el premio Turing, considerado el premio Nobel de la Informática. Wilkes bautizó a las agrupaciones de código con el nombre de subrutinas, pero posteriores lenguajes de programación les han ido dando distintos nombres (subrutinas, procedimientos, funciones, métodos, etc.) y dándoles distintas características.

Las subrutinas tienen muchas ventajas evidentes:

ahorrar trabajo: si sabemos cómo realizar una tarea, no es necesario volver a programarla una y otra vez.
facilitar el mantenimiento: si descubrimos errores en una subrutina, sólo hay que corregirlos en un sitio, sin tener que recordar en cuántos sitios utilizamos el algoritmo.
simplificar el código: la longitud y complejidad del programa se reducen porque las tareas repetitivas ya no aparecen en el cuerpo del programa.
facilitar la creación de programas: el trabajo se puede dividir entre varios programadores (unos escriben las subrutinas, otros el cuerpo principal del programa, etc.).
Si una subrutina se va a utilizar en un único programa, se suele definir en el propio programa. Pero cuando una subrutina se va a utilizar en varios programas, no es necesario repetirla en cada programa (se perderían algunas de las ventajas comentadas anteriormente), sino que se puede incluir en un fichero aparte al que los programas pueden acceder para recuperar las subrutinas. Estos ficheros reciben el nombre de bibliotecas (en español se suele decir mucho librería, traduciendo incorrectamente el término inglés library).

En Python se utiliza el término función para referirse a las subrutinas y el término módulo para referirse a las bibliotecas.

Última modificación de esta página: 4 de marzo de 2016

##El if

El programa siguiente pide un número positivos al usuario y almacena la respuesta en la variable "numero". Después comprueba si el número es negativo. Si lo es, el programa avisa que no era eso lo que se había pedido. Finalmente, el programa imprime siempre el valor introducido por el usuario. A continuación se pueden ver dos ejecuciones paso a paso de ese programa. En la primera el usuario escribe un valor negativo y en la segunda el usuario escribe un valor positivo:

Ejemplo de if ... 1

numero = int(input("Escriba un número positivo: "))

if numero < 0:

print("¡Le he dicho que escriba un número positivo!")

print(f"Ha escrito el número {numero}")

Escriba un número positivo: -5

¡Le he dicho que escriba un número positivo!

Ha escrito el número -5

Puede ver la ejecución paso a paso de este programa utilizando los iconos de avance y retroceso situados abajo a la derecha.
 
Ejemplo de if ... 1 - Paso 1

numero = int(input("Escriba un número positivo: "))

if numero < 0:

print("¡Le he dicho que escriba un número positivo!")

print(f"Ha escrito el número {numero}")

Escriba un número positivo: -5

Se ejecuta la primera instrucción del programa.

Ejemplo de if ... 2
numero = int(input("Escriba un número positivo: "))
if numero < 0:
    print("¡Le he dicho que escriba un número positivo!")
print(f"Ha escrito el número {numero}")
Escriba un número positivo: 5
Ha escrito el número 5
Puede ver la ejecución paso a paso de este programa utilizando los iconos de avance y retroceso situados abajo a la derecha.
 
Ejemplo de if ... 2 - Paso 1
numero = int(input("Escriba un número positivo: "))
if numero < 0:
    print("¡Le he dicho que escriba un número positivo!")
print(f"Ha escrito el número {numero}")
Escriba un número positivo: 5
Se ejecuta la primera instrucción del programa.
En este caso, imprime la pregunta y espera a que el usuario escriba la respuesta y pulse Intro, guardando la respuesta en la variable "numero".
   
Ejemplo de if ... 2 - Paso 2
numero = int(input("Escriba un número positivo: "))
if numero < 0:
    print("¡Le he dicho que escriba un número positivo!")
print(f"Ha escrito el número {numero}")
Escriba un número positivo: 5
A continuación se evalúa la condición (numero < 0).
En este caso, la condición es falsa (False), puesto que 5 no es inferior a 0.
   
Ejemplo de if ... 2 - Paso 3

numero = int(input("Escriba un número positivo: "))

if numero < 0:

print("¡Le he dicho que escriba un número positivo!")

print(f"Ha escrito el número {numero}")

Escriba un número positivo: 5

Ha escrito el número 5

Como la condición es falsa, no se ejecutan las instrucciones del bloque y el programa salta a la instrucción siguiente al bloque if ..

La última instrucción del programa imprime el valor introducido y el programa termina.

La estructura de control if ... else ... permite que un programa ejecute unas instrucciones cuando se cumple una condición y otras instrucciones cuando no se cumple esa condición. En inglés "if" significa "si" (condición) y "else" significa "si no". La orden en Python se escribe así:

Sintaxis de la sentencia condicional if ... else ...

La sintaxis de la construcción if ... else ... es la siguiente:

if condición:

aquí van las órdenes que se ejecutan si la condición es cierta

y que pueden ocupar varias líneas

else:

y aquí van las órdenes que se ejecutan si la condición es

falsa y que también pueden ocupar varias líneas

La ejecución de esta construcción es la siguiente:

•	La condición se evalúa siempre.

o	Si el resultado es True se ejecuta solamente el bloque de sentencias 1

o	Si el resultado es False se ejecuta solamente el bloque de sentencias 2.

Más de dos alternativas: if ... elif ... else ...

La construcción if ... else ... se puede extender añadiendo la instrucción elif:
La estructura de control if ... elif ... else ... permite encadenar varias condiciones. elif es una contracción de else if. La orden en Python se escribe así:

Sintaxis de la sentencia condicional if ... elif ... else ...
La sintaxis de la construcción if ... elif ... else ... es la siguiente:

if condición_1:

bloque 1

elif condición_2:

bloque 2

else:

bloque 3

•	Si se cumple la condición 1, se ejecuta el bloque 1

•	Si no se cumple la condición 1 pero sí que se cumple la condición 2, se ejecuta el bloque 2

•	Si no se cumplen ni la condición 1 ni la condición 2, se ejecuta el bloque 3.

##El bucle for
En general, un bucle es una estructura de control que repite un bloque de instrucciones. Un bucle for es un bucle que repite el bloque de instrucciones un número prederminado de veces. El bloque de instrucciones que se repite se suele llamar cuerpo del bucle y cada repetición se suele llamar iteración.

La sintaxis de un bucle for es la siguiente:

for variable in elemento iterable (lista, cadena, range, etc.):

cuerpo del bucle

No es necesario definir la variable de control antes del bucle, aunque se puede utilizar como variable de control una variable ya definida en el programa.

El cuerpo del bucle se ejecuta tantas veces como elementos tenga el elemento recorrible (elementos de una lista o de un range(), caracteres de una cadena, etc.). Por ejemplo:

Ejemplo de bucle 1

print("Comienzo")

for i in [0, 1, 2]:

print("Hola ", end="")

print()

print("Final")

Comienzo

Hola Hola Hola

Final

Puede ver la ejecución paso a paso de este programa utilizando los iconos de avance y retroceso situados abajo a la derecha.

La lista puede contener cualquier tipo de elementos, no sólo números. El bucle se repetirá siempre tantas veces como elementos tenga la lista y la variable irá tomando los valores de uno en uno. Por ejemplo:

Ejemplo de bucle 6

print("Comienzo")

for i in ["Alba", "Benito", 27]:

print(f"Hola. Ahora i vale {i}")

print("Final")

Comienzo

Hola. Ahora i vale Alba

Hola. Ahora i vale Benito

Hola. Ahora i vale 27

Final

El ciclo while esta hecho para condicionar una parte del codigo y mientras no se cumpla el codigo se erepita la instruccion

El siguiente programa escribe los números del 1 al 3:

Ejemplo de bucle while 1

i = 1

while i <= 3:

print(i)

i += 1

print("Programa terminado")

1

2

3

Programa terminado

 ## El módulo turtle
 
 Python incluye un módulo llamado "turtle" que permite crear gráficos de tortuga.

En esta lección se explica cómo utilizar el módulo turtle para crear dibujos sencillos, pero sin utilizar la tortuga.

Para utilizar el módulo turtle sólo hace falta importarlo:

Si se va a escribir código orientado a objetos:
import turtle

La ventana de dibujo: setup() y title()
El módulo turtle dibuja en una ventana distinta a la ventana de IDLE. Esta ventana de dibujo se crea al ejecutar un programa y se mantiene al acabar la ejecución del programa, pero se destruye al volver a ejecutar el programa).

La función setup(ancho, alto, posicionX, posicionY) permite definir el tamaño y la posición inicial de la ventana. Los cuatro argumentos de la función son (en píxeles):


ancho: ancho de la ventana.

alto: alto de la ventana.

posicionX: posición horizontal de la ventana. Los valores positivos se miden desde el borde izquierdo de la pantalla, los negativos 
desde el borde derecho de la pantalla.

posicionY: posición vertical de la ventana. Los valores positivos se miden desde el borde superior de la pantalla, los negativos desde el borde inferior de la pantalla.

La función title() permite definir el título de la ventana, que se muestra en el borde superior de la ventana.

from turtle import *

setup(450, 150, 0, 0)
title("Ejemplo de ventana")

Si no se usa la función setup(), la ventana se crea en el centro de la pantalla (para que se cree la ventana tiene que aparecer alguna función del módulo turtle):

from turtle import *

title("Ejemplo de ventana")

mainloop()

Para crear programas de tortuga interactivos necesitamos que los programas no terminen, sino que permanezcan a la espera y reaccionen a los eventos (de ratón o de teclado) generados por el usuario.

La función mainloop(), que se escribe al final del programa, hace que el programa no termine, sino que permanezca a la espera de los eventos definidos en el programa.
