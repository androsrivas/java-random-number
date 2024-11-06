# Recursos Java 

## Arrays
Un array, también conocido como arreglo o vector, es una estructura de datos que permite almacenar una colección de elementos del mismo tipo en una ubicación contigua de memoria. Los elementos de un array se acceden mediante índices, que son números enteros que indican la posición del elemento dentro del array. Los índices generalmente comienzan en 0 para la mayoría de los lenguajes de programación. Su sintaxis es la siguiente:

String[] greeting = {"hola", "hello", "salut"};

### Reglas
- No se puede cambiar el largo de un array
- Almacena datos pero tienen que ser del mismo tipo

### Print arrays:
- Se llama a la clase Arrays, al método toString del paquete de java.util:
System.out.println(Arrays.toString(array)); 
- También se puede hacer un bucle e imprimir por item  

### Bucle for each 
El bucle 'for-each' en Java es una estructura de control diseñada para iterar de manera eficiente sobre todos los elementos de un array. Simplifica la sintaxis y hace que el código sea más legible en comparación con los bucles 'for' tradicionales. En lugar de usar índices para acceder a cada elemento, el bucle 'for-each' permite trabajar directamente con los elementos del array.

int[] numeros = {1, 2, 3, 4, 5};

for (int numero : numeros) {
    System.out.println(numero);
}

### The Reference Trap
No se debe igualar una variable a otra variable que contenga un array porque se quedan enlazados entre ellos, ya que la nueva variable coge la referencia del anterior.

String[] trabajadores2023 = {"Tommy", "Joel", "Ellie"};
String[] trabajadores2024 = trabajadores2023;

Si quiero modificar el valor del índice 0 del segundo array se modificará también el valor del índice 0 del primer array.

- Lo mejor será hacer un nuevo array, creando uno nuevo o usando el método copy de la clase Arrays del paquete java.util


* Arrays
https://www.w3schools.com/java/java_arrays.asp

* For-each
https://www.w3schools.com/java/java_arrays_loop.asp

* Arrays Multidimensionales 
https://www.w3schools.com/java/java_arrays_multi.asp


