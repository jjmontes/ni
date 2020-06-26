# Ni

<img src="https://raw.githubusercontent.com/DeybisMelendez/ni/master/logo.jpg" width="300"/>

English description in: https://esolangs.org/wiki/Ni

## ¿Qué es Ni?
Ni es un lenguaje de programación esotérico escrito en Lua influenciado por Brainfuck. El nombre Ni viene de Nicaragua.

## ¿Cómo funciona?

Ni opera con un arreglo de números enteros, en referencia a la cinta de la máquina de Turing al igual que brainfuck, contiene un total de 65,536 celdas que se inicializan en cero. Cada celda contiene un número entero de 64 bits.

Ni tiene un cabezal que apunta a la memoria de una celda del array que puedes manipular con instrucciones.

Ni también maneja un clipboard, como una variable global a la que se puede acceder y modificar en cualquier momento.

## Instrucciones

|Instrucción|Descripción |
|-----------|------------|
|>          |Mueve el cabezal a la derecha |
|<          |Mueve el cabezal a la izquierda|
|+          |Suma 1 al número de la celda apuntada|
|-          |Resta 1 al número de la celda apuntada|
|@          |Lee el primer caracter, lo convierte a su número ASCII y lo almacena en la celda apuntada|
|.          |Imprime en pantalla el número almacenado en la celda apuntada|
|!          |Imprime en pantalla el equivalente ASCII del número almacenado en la celda apuntada|
|#          |Establece un valor hexadecimal de dos dígitos en la celda apuntada|
|?          |Copia el número de la celda apuntada|
|=          |Almacena el número copiado en la celda apuntada|
|*          |Convierte a 0 el número de la celda apuntada|
|$          |Mueve el cabezal hacia el indice del número hexadecimal de 4 digitos que se escriba a continuación|
|[]         |(While) Bucle que continua ejecución si la celda apuntada no es igual a 0|
|{}         |(For) Bucle que ejecuta las instrucciones el número de veces que indica la memoria de la celda apuntada|
|()         |(if) Ejecuta el conjunto de instrucciones si el número apuntado no es igual a 0|
|/          |Ignora el resto de la línea|

## Como ejecutar

Descarga Ni aquí: https://github.com/DeybisMelendez/ni/releases

### Windows

Coloca el ejecutable al lado del script con formato **.ni**
Abre el CMD y ejecuta **ni tucodigo.ni**

### Linux

Coloca el ejecutable al lado del script con formato **.ni**
Abre la terminal y ejecuta **./ni tucodigo.ni**

### Con Lua 5.2

Coloca el main.lua junto al script con formato **.ni**
Abre la terminal o CMD y ejecuta **lua main.lua tucodigo.ni**

## Ejemplos

### Hola Mundo!

Este código imprime el hola mundo.

#48!#6f!#6c!#61!#20!#4d!#75!#6e!#64!#6f!#21!#0a!

### Cat

Este código imprime devuelta el byte que escribas

#01[@!#0a!]

Hay mas ejemplos en la carpeta *examples*.

## Envía ejemplos

El objetivo principal de programar en Ni es la diversión, el desafío de crear un programa que funcione, en la carpeta *examples* se recopilan estos programas.

Puedes enviar pull requests si escribes uno, enviarlo como un issue o en Discord para añadirlo.

Hay una serie de problemas populares para resolver y mostrar la capacidad de un lenguaje de programación esotérico, la lista está aquí: https://esolangs.org/wiki/Popular_problem

Los principales problemas a resolver son:

- Programa que calcule el factorial de un dígito. (agregado por usuario de Discord Jjony#5227)
- Programa que imprima la sucesión de [Thue-Morse](https://es.wikipedia.org/wiki/Sucesi%C3%B3n_de_Thue-Morse) o cualquier otra sucesión conocida.
- Programa que imprima el [Triangulo de Sierpinski](https://es.wikipedia.org/wiki/Tri%C3%A1ngulo_de_Sierpinski).
- Programa que haga [Quine](https://es.wikipedia.org/wiki/Quine_(programa)).

Además, añado estos:

- Programa que ejecute el [Juego de la vida](https://es.wikipedia.org/wiki/Juego_de_la_vida).
- Programa que ejecute la [Hormiga de Langton](https://es.wikipedia.org/wiki/Hormiga_de_Langton).

## Próximamente

Añadir un sistema de errores comunes.

## Discord

He creado un servidor en Discord, participa en el chat con este enlace: https://discord.gg/dxYxZs5
