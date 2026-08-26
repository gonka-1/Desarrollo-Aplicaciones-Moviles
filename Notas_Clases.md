# Desarrollo-Aplicaciones-Moviles


val a = Int = 1// Inmutable // Constante
var b = Int = 2//Mutable // Variable

Estructura básica de un programa:

Print de Kotlin:

fun main(){
	println("Hello, World!")
}

Ejemplo con Variables

fun main() {
    
    val run : String = "123456789-0"
    var nombre: String = "Pedro"
    
    nombre = "Juan Pedro"
    
    println("run: " + run + "\nNombre: " + nombre)
    
}

//se le añade (?) para que la variable sea declarada nula
var a: String? = "Hello" 
a = null

//se le añade (!!) para que la variable sea declarada no-nula
var a: String!! = "Hello" 


///Nota: Todos los valores son con la primera letra en mayúscula(String, Int, Double, boolean)

--Deferencia entre Int y Double: Int son números enteros más pequeños(14) y Double almacena números enteros más grandes(140000000).

--Modulo: Entrega el número que sobra cuando hacemos una división (5 % 2 = 1).

\\\

Los arreglos tienen un orden A = [1, 2, 3]. 

- Listas(LIST): Colecciones ordenadas que pueden contener elementos duplicados.

val numeros = listof(1,2,3) -- inmutable
val lista = mutableListof(1,2,3) lista.add(4) --mutable

- Conjuntos (SET): Colecciones de elementos únicos que no permiten duplicados y no tienen orden.

val conjunto = setOf(1, 2, 3) --inmutable
val conjunto = mutableSetOf("a", "b") conjunto.add("c") --mutable.

- Mapas(MAP): Colecciones de pares clave-valor que asocian claves únicas con valores (Diccionarios). 

val mapa = mapOf("a" to 1, "b" to 2) --inmutable
val mapa = mutableMapOf("Nombre" to "Jose") mapa["apellido"] = "Rojo"


- Filtrado de colecciones: 
val numeros = listof(1,2,3, 4, 5, 6)
val n = numeros.filter{it % 2 == 0}
prinln(n) // [2, 4, 6]

- Mapeo de colecciones: (Operaciones para una lista completa)

val n = numeros.map{it * 2}
println(n)//[2, 4, 6, 8, 10, 12]

- Reducción de colecciones(reduce): Combina todos los elementos de una lista en un solo valor.

val sum = numeros.reduce{acc, numero -> acc + numero}
println(sum) // 21

- Búsqueda de colecciones: Puedes buscar elementos en una colección utilizando funciones como find, first last, etc.

val n = numeros.find{it % 2 == 0}
println(n)//2

- **Opciones Avanzadas:**
  
- Agrupacion: Puedes agrupar elementos de una colección basandote en un criterio.

  val numeros = listOf(1, 2, 3, 4, 5, 6, 6, 6, 5, 3)
  val grupoPares = numeros.groupBy{it % 2 == 0}
  println("gruposPares: " + grupoPares)
  
- Ordenación: Las colecciones se pueden ordenar utilizando sortedBy o sortedDescending
  
  val numeros 		= listOf(1, 2, 3, 4, 5, 6, 6, 6, 5, 3)
  val ordenAscenso = numeros.sorted() // Ascenso
  val ordenDescenso = numeros.sortedDescending() // Descenso
  println("ordenAscenso: " + ordenAscenso)
  println("ordenDescenso: " + ordenDescenso)


  - Kotlin como lenguaje:

  Objeto -> Instancia de Clase -> Parámetros(Atributos) y funciones(Acciones)

  **4 principios de desarrollo orientado a objetos:**

  - Herencia: las clases hijas heredan las funciones de la clase padre.
  - Abstracción: simplificar las características de la clase.
  - Encapsulamiento: Ocultar los datos de la clase.
  - Polimorfismo: Dos objetos pueden tener la misma funcón pero se comportan de forma distinta.
 
- **Constructor**: pide los parametros(atributos) para crear una instacia de una clase.

**SOLID**: es un grupo de cinco reglas de diseño para la Programación Orientada a Objetos. Ayudan a crear código limpio, fácil de leer, cambiar y ampliar sin romper otras partes del programa.
  
- S (Responsabilidad Única): Una clase hace una sola tarea y tiene una sola razón para cambiar.
- O (Abierto/Cerrado): El código acepta nuevas funciones sin modificar lo que ya funciona.
- L (Sustitución de Liskov): Las clases hijas reemplazan a las clases padres sin causar fallos.
- I (Segregación de Interfaces): Es mejor tener varias interfaces pequeñas que una sola muy grande y pesada.
- D (Inversión de Dependencias): Los módulos dependen de abstracciones y no de detalles concretos

- Corrutinas: Son la forma idiomática de Kotlin para manejar tareas asíncronicas. Piensa en ellas como hilos súper ligeros.
  
- Apply: para configurar o inicializar un objeto, permitiendo modificar sus propiedades y luego devolver el mismo objeto ya modificado.

- Let: sirve para ejecutar un bloque de código sobre un objeto de manera segura y ordenada, usando it para referirse a él y devolviendo el resultado de la última línea.

***Compilador de java gratuito: https://onecompiler.com/java***

***Compilador de Kotlin gratuito: https://play.kotlinlang.org/***
