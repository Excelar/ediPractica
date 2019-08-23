# JavaScript

![N|Solid](https://techtatva.co/techtatva140717/wp-content/uploads/2018/09/js-logo-465x465.png)

## Qué es JavaScript

  JavaScript(abreviado comúnmente JS) es un lenguaje de programación interpretado, dialecto del estándar ECMAScript. Se define como orientado a objetos, basado en prototipos, imperativo, débilmente tipado y dinámico.
Se utiliza principalmente en su forma del lado del cliente (client-side), implementado como parte de un navegador web permitiendo mejoras en la interfaz de usuario y páginas web dinámicas aunque existe una forma de JavaScript del lado del servidor(Server-side JavaScript o SSJS). 

## Para qué se puede usar JavaScript

- OpenSource Projects: [OpenLayers](https://openlayers.org/), [jQuery](https://jquery.com/), [Bootstrap 4](https://getbootstrap.com/), [Mozilla Firefox](https://www.mozilla.org/es-AR/firefox/new/), [React JS](https://es.reactjs.org/), [Grunt](https://gruntjs.com/)

- WebBrowser: [Google Chrome](https://www.google.com), [Mozilla Firefox](https://www.mozilla.org/es-AR/firefox/new/)

- Apps: [Skype](https://www.skype.com), [Mozilla Thunderbird](https://www.thunderbird.net), [Spotify](https://www.spotify.com)

# Dónde se usa JavaScript

JavaScript es un lenguaje de programación, al igual que PHP, si bien tiene diferencias importantes con éste. JavaScript se utiliza principalmente del lado del cliente (es decir, se ejecuta en nuestro ordenador, no en el servidor) permitiendo crear efectos atractivos y dinámicos en las páginas web. Los navegadores modernos interpretan el código JavaScript integrado en las páginas web.

Para entender lo que es JavaScript consideremos lo siguiente. Un usuario escribe una dirección web en su navegador, por ejemplo http://www.aprenderaprogramar.com. El servidor recibe la petición y como respuesta a esa petición envía al ordenador del usuario código HTML junto a código JavaScript. El código HTML se encarga de que en la pantalla se muestre algo, por ejemplo una imagen, un menú, etc. El código JavaScript se puede encargar de crear efectos dinámicos en respuesta a acciones del usuario, por ejemplo que se despliegue un menú tipo acordeón cuando el usuario pasa el ratón por encima de un elemento del menú.

La ventaja de JavaScript es que al estar alojado en el ordenador del usuario los efectos son muy rápidos y dinámicos. Al ser un lenguaje de programación permite toda la potencia de la programación como uso de variables, condicionales, bucles, etc. También podemos citar algún inconveniente: por ejemplo si el usuario tiene desactivado JavaScript en su navegador, no se mostrarán los efectos. No obstante, hoy día la mayoría de los usuarios navegan por la web con JavaScript activado.

### Instalación

En linux:
La mayoría de las distribuciones de Linux no soportan JavaScript pero usan la librería Node.js en su lugar.
Abrir una consola y escribir:
```sh
$ sudo apt-get install nodejs
```
En Windows ya viene preinstalado, pero para su desarrollo cualquier IDE con compatibilidad con JS funciona de maravilla(ATOM, Eclipse con JSDT)


## Micro Tutorial de JS

#### Comentarios

El lenguaje Javascript tiene una sintaxis muy parecida a la de Java por estar basado en él. También es muy parecida a la del lenguaje C, de modo que si el lector conoce alguno de estos dos lenguajes se podrá manejar con facilidad con el código. De todos modos, en los siguientes capítulos vamos a describir toda la sintaxis con detenimiento, por lo que los novatos no tendrán ningún problema con ella.
Comentarios en el código. Un comentario es una parte de código que no es interpretada por el navegador y cuya utilidad radica en facilitar la lectura al programador. El programador, a medida que desarrolla el script, va dejando frases o palabras sueltas, llamadas comentarios, que le ayudan a él o a cualquier otro a leer mas fácilmente el script a la hora de modificarlo o depurarlo.

Existen dos tipos de comentarios en el lenguaje. 
Uno de ellos, la doble barra, sirve para comentar una línea de código. 
El otro comentario lo podemos utilizar para comentar varias líneas y se indica con los signos /* para empezar el comentario y */ para terminarlo. 
Veamos unos ejemplos.

><SCRIPT>

>//Este es un comentario de una línea

>/*Este comentario se puede extender

>por varias líneas.

>Las que quieras*/

></SCRIPT>

Mayúsculas y minúsculas

En Javascript se han de respetar las mayúsculas y las minúsculas. 
Si nos equivocamos al utilizarlas el navegador responderá con un mensaje de error, ya sea de sintaxis o de referencia indefinida.

#### Variables

>sumando1 = 23 

>sumando2 = 33 

>suma = sumando1 + sumando2


En este ejemplo tenemos tres variables, sumando1, sumando2 y suma, donde guardamos el resultado. Vemos que su uso para nosotros es como si tuviésemos un apartado donde guardar un dato y que se pueden acceder a ellos con sólo poner su nombre.

Los nombres de las variables han de construirse con caracteres alfanuméricos y el carácter subrayado (_). Aparte de esta, hay una serie de reglas adicionales para construir nombres para variables. La más importante es que tienen que comenzar por un carácter alfabético o el subrayado. No podemos utilizar caracteres raros como el signo +, un espacio o un $. Nombres admitidos para las variables podrían ser:

>Edad

>paisDeNacimiento

>_nombre


También hay que evitar utilizar nombres reservados como variables, por ejemplo no podremos llamar a nuestra variable palabras como return o for, que ya veremos que son utilizadas para estructuras del propio lenguaje. Veamos ahora algunos nombres de variables que no está permitido utilizar:

>12meses

>tu nombre

>return

>pe%pe

#### Declaración de variables en Javascript

Declarar variables consiste en definir y de paso informar al sistema de que vas a utilizar una variable. Es una costumbre habitual en los lenguajes de programación el definir las variables que se van a usar en los programas y para ello, se siguen unas reglas estrictas. Pero Javascript se salta muchas reglas por ser un lenguaje un tanto libre a la hora de programar y uno de los casos en los que otorga un poco de libertad es a la hora de declarar las variables, ya que no estamos obligados a hacerlo, al contrario de lo que pasa en la mayoría de los lenguajes de programación.

Javascript cuenta con la palabra "var" que utilizaremos cuando queramos declarar una o varias variables. Como es lógico, se utiliza esa palabra para definir la variable antes de utilizarla.
Nota: Aunque Javascript no nos obligue a declarar explícitamente las variables, es aconsejable declararlas antes de utilizarlas y veremos en adelante que se trata también de una buena costumbre. Además, en sucesivos artículos veremos que en algunos casos especiales, no producirá exactamente los mismos resultados un script en el que hemos declarado una variable y otro en el que no lo hagamos.

>var operando1

>var operando2


También se puede asignar un valor a la variable cuando se está declarando

>var operando1 = 23

>var operando2 = 33

También se permite declarar varias variables en la misma línea, siempre que se separen por comas.

>var operando1,operando2

##### Tipo de datos numérico

En este lenguaje sólo existe un tipo de datos numérico, al contrario que ocurre en la mayoría de los lenguajes más conocidos. Todos los números son por tanto del tipo numérico, independientemente de la precisión que tengan o si son números reales o enteros. Los números enteros son números que no tienen coma, como 3 o 339. Los números reales son números fraccionarios, como 2.69 o 0.25, que también se pueden escribir en notación científica, por ejemplo 2.482e12.

Con Javascript también podemos escribir números en otras bases, como la hexadecimal. Las bases son sistemas de numeración que utilizan más o menos dígitos para escribir los números. Existen tres bases con las que podemos trabajar

    Base 10, es el sistema que utilizamos habitualmente, el sistema decimal. Cualquier número, por defecto, se entiende que está escrito en base 10.
    Base 8, también llamado sistema octal, que utiliza dígitos del 0 al 7. Para escribir un número en octal basta con escribir ese número precedido de un 0, por ejemplo 045.
    Base 16 o sistema hexadecimal, es el sistema de numeración que utiliza 16 dígitos, los comprendidos entre el 0 y el 9 y las letras de la A a la F, para los dígitos que faltan. Para escribir un número en hexadecimal debemos escribirlo precedido de un cero y una equis, por ejemplo 0x3EF.

##### Tipo boleano

El tipo bolean, boolean en inglés, sirve para guardar un si o un no o dicho de otro modo, un verdadero o un falso. Se utiliza para realizar operaciones lógicas, generalmente para realizar acciones si el contenido de una variable es verdadero o falso.

> Si una variable es verdadero entonces ----- Ejecuto unas instrucciones

> Si no ----- Ejecuto otras

Los dos valores que pueden tener las variables boleanas son true o false.

> miBoleana = true

> <br>

> miBoleana = false

##### Tipo de datos cadena de caracteres 

El último tipo de datos es el que sirve para guardar un texto. Javascript sólo tiene un tipo de datos para guardar texto y en el se pueden introducir cualquier número de caracteres. Un texto puede estar compuesto de números, letras y cualquier otro tipo de caracteres y signos. Los textos se escriben entre comillas, dobles o simples.

> miTexto = "Pepe se va a pescar" 

> miTexto = '23%%$ Letras & *--*'

Todo lo que se coloca entre comillas, como en los ejemplos anteriores es tratado como una cadena de caracteres independientemente de lo que coloquemos en el interior de las comillas. Por ejemplo, en una variable de texto podemos guardar números y en ese caso tenemos que tener en cuenta que las variables de tipo texto y las numéricas no son la misma cosa y mientras que las de numéricas nos sirven para hacer cálculos matemáticos las de texto no.
Caracteres de escape en cadenas de texto

Hay una serie de caracteres especiales que sirven para expresar en una cadena de texto determinados controles como puede ser un salto de línea o un tabulador. Estos son los caracteres de escape y se escriben con una notación especial que comienza por una contra barra (una barra inclinada al revés de la normal '') y luego se coloca el código del carácter a mostrar.

Un carácter muy común es el salto de línea, que se consigue escribiendo n. Otro carácter muy habitual es colocar unas comillas, pues si colocamos unas comillas sin su carácter especial nos cerrarían las comillas que colocamos para iniciar la cadena de caracteres. Las comillas las tenemos que introducir entonces con " o ' (comillas dobles o simples). Existen otros caracteres de escape, que veremos en la tabla de abajo más resumidos, aunque también hay que destacar como carácter habitual el que se utiliza para escribir una contrabarra, para no confundirla con el inicio de un carácter de escape, que es la doble contrabarra .
Tabla con todos los caracteres de escape

> Salto de línea: \n

> Comilla simple: \'

> Comilla doble: \"

> Tabulador: \t

> Retorno de carro: \r

> Avance de página: \f

> Retroceder espacio: \b

> Contrabarra: \\

Algunos de estos caracteres probablemente no los llegarás a utilizar nunca, pues su función es un poco rara y a veces poco clara. 
