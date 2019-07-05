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

