# Aqui vamos a hablar de tipos de datos (data types) principales.

`package com.usauriorawr.usaurioRAWR_Leccion2TiposDeDatos`

~~~
import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
~~~

~~~
class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

    // Leccion 2
        tiposDeDatos()
    }
~~~

`private fun tiposDeDatos() {`


> El tipo de dato definira el valor que puede adoptar nuestra variable o constante y las operaciones que se podran realizar con dichpos datos.

> ### String (Cadena)
>
>Este tipo de dato va a representar una cadena de texto.

~~~
        val myString1 = "Hola myString"`
~~~

> -. Como podemos observar en nungun momento hemos indicado que la variable es de tipo String.
> Sin embargo Kotlin es capaz de identificar el tipo de dato unicamente por como se representa,
> gracias a su caracteristica "La diferencia de tipos".
>
> -. En el caso de String; cualquier cadena de texto tiene que ir entre comillas dobles simples(" "),
> por lo que kotlin automaticamente deduce y declara que la variable o constante es de tipo String.

> +. Seria lo mismo que nosotros a continuacion de la variablle o constante pusieramos "dos
> puntos + espacio + palabra reserbada para el tipo de dato"
> 
>       -. Ej.
>           /~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\
>           |val myString: String = "Hola myString"|
>           \~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~/
>           -. Pero; Android Studio nos diria que la declaracion es redundante ya que el lo deduce.

~~~
        val myString2 = "Biembenido a Kotlin"
~~~

>  #### Operaciones que podemos realizar con los datos de tipo String.;
>            +. Juntarlos / sumerlos.
>                +. Sintaxis;
>                    -. val nombreDeLaNuevaVariable = variableAJuntar + variableASumar
>                +. Ej.
>                   +. Entrada;
>                        val myString3 = myString1 + myString2
>                    +. Salida;
>                        Hola myStringBiembenido a Kotlin>
>                        
>                +. Para crear un espacion entre las dos variables sumaremos <" "> entre las dos.
>                    +. Ej.
>                       /~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\
>                       |val myString3 = myString1 + " " + myString2|
>                       \~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~/

~~~
    val myString3 = myString1 + " " + myString2
    println(myString3)
~~~


> ### Enteros (Byte, Short, Int, Long)
>
> #### Tipos de numeros enteros (4).
> 
>        +. La unica diferencia entre los cuatro tipos de numeros enteros, es la longitud del numero
> que pueden albergar .
>            -. Byte; Numeros entre -127 y 128.
>            -. Short; Numeros entre -32.768 y 32.767
>            -. Int; Numeros entre -2.147.483.647 y 2.147.483.647
>            -. Long; Numeros entre -9.223.372.036.854.775.807 a 9.223.372.036.854.775.807
>
>        -. La recomendacion es utilizar el tipo de dato que mejor se adapte "a la posible
> longitud", para que asi ocupe menos en memoria.
>
>        -. Lo mas normal es trabajar casi siempre con numeros enteros de tipo Int y cuando
>son muy muy grandes, de tipo long

~~~
    val myInt = 1 // Kotlin dara siempre por sentado que es de tipo Int.
    val myInt2 = 2
    val myInt3 = myInt + myInt2
    println(myInt3)
~~~


> ### Decimales (Float; 32bits, Double; 64bits)
    
~~~
    val myDouble = 1.5
~~~

> La diferencia de tipos siempre establecera que es de tipo Double.
> Y para indicar que es de tipo Float se debe de hacer asi.
    
~~~
val myFloat: Float = 1.5f
~~~
    
~~~
    val myDouble2 = 1.6
~~~
    
> Numero entero de tipo Int.↴
    
~~~
    val myDouble3 = 2
~~~
    
> La diferencias de tipo asignara el resultado de "myDouble4" como de tipo de tipo Double.
> En la suma decimal hay una variable que con un valor entero "myDouble3", lo que
> sucedera es que el sistema internamente lo convertira en un numero decimal 2 > 2.0
    
~~~
    val myDouble4 = myFloat + myDouble2 + myDouble3
    println(myDouble4)
    val myDouble5 = myDouble - myDouble3 // La diferencias de tipo asignara Double.
    println(myDouble5)
    val myDouble6: Double = myDouble - myDouble3 // Se establece que sea de tipo Double.
    println(myDouble6)
~~~

//---------------------------------------------------Decimales (Float; 32bits, Double; 64bits) <Fin>

// <Inicio> Boolean (Bool, Describe condiciones; verdadera o flasa)---------------------------------
    val myBool = true
    val myBool2 = false
    // Los valores booleanos solo aceptan operaciones logicas.
    println(myBool && myBool2)
    println(myBool || myBool2)
/*:-------------------------------------------------------------------------------------------------
Errores;

        /~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\
    +.  |val myBool3 = myBool + myBool2|
        \~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~/
        -. Dara error ya que no es una operacion logica.
 */
/*
    +. Las operaciones logicas son;
        -. AND (multiplicacion) y se indica con dos iguales "&&"
        -. OR (suma) y se indica con dos ampersand "||".
 */
//-------------------------------------Boolean (Bool, Describe condiciones; verdadera o flasa) <Fin>
}

// :-----------------------------------------------------------------------------------------------:
// (Fin) Aqui terminamos de hablar de tipos de datos (data types) principales.----------------------
// :-----------------------------------------------------------------------------------------------:



}
