## 2. 
### Para preprocesar el archivo hello2.c utilice el siguiente comando en la consola "cgg -E hello2.c", este comando me mostro el resultado por pantalla, en el cual se podia contemplar que el comentario "/*medio*/" se habia remplazado por un espacio, generando una correcta sintaxis.
### Para generar el archivo Hello2.i utilice el comando "cgg hello2.c -E > hello2.i"

## 4. es la declaracion de una funcion quetiene como salida un stdout de una cadena de caracteres

## 5. 
### Para preprocesar el archivo hello3.c utilice el siguiente comando en la consola "cgg -E hello3.c". Para generar el archivo Hello2.i utilice el comando "cgg hello3.c -E > hello3.i"
### En el archivo hello3.i se agregaron siguientes lineas al principio del archivo:
#### # 1 "hello3.c"

#### # 1 "<built-in>"
 
#### # 1 "<command-line>"

#### # 1 "hello3.c" "

## 6.

### Para compilar el archivo hello3.c utilice el siguiente comando en la consola "cgg -S hello3.c" y se genero el archivo hello3.s sin ensamblarse. Genera un error sintaxis, ya que falta una } para cerrar el mail.

## 7.
### Las correcciones hechas en hello3.c para generar hello4.c fueron:
#### Agregar la } faltante para cerrar el main
### Utilice los comandos "cgg -E hello4.c" para generar el preprocesado y el comando "cgg -S hello4.c" para ensamblar

## 8.
### En el archivo hello.s se remplazo todo el lenguaje de alto nivel por lenguaje de bajo nivel (assembler).
### Como en lenguaje de bajo nivel no existe una operacion para printf, se genero una linea al final del archivo:
#### "	.def	printf;	.scl	2;	.type	32;	.endef" 

## 9.
### Para ensamblar el archivo hello4.s en hello4.o sin vincular, utilice el comando " as -o hello4.o hello4.s

## 10.
### Para enlazar el archivo hello4.o con la biblioteca estandar, el comando utilizado fue: "gcc hello4.o -LStandard

## 11.
### El arreglo realizado para el archivo hello5.c fue:
### se remplazo prontf por printf
#### Se agrego la funcion "getchar();" para que el programa espere a recibir una tecla para continuar y asi ver por pantalla el resultado, ya que al terminar la sentencia, el programa se cerraba

## 12.
### Hello5 no muestra el resultado correcto por pantalla, ya que nunca se le pasa la variable i, la cual contiene almacenada el numero 42.

#### El resultado es "La respuesta es 8683848483", este ultimo numero cambiaba cada vez que se ejecutaba el programa, el cual es informacion desconocida

## 13.
### EL arreglo realizado para el achivo hello6.c fue:
#### Modificar "printf("La respuesta es %d\n");" por "printf("La respuesta es %d\n",i);" para que recibiera la varible i que contenia almacenada el numero que se requerria mostar por pantalla.

#### El resultado final fue "La respuesta es 42"

## 14.
### Funciona ya que C permite generar declaraciones implicitas.
