# Aqui vamos a hablar de variables y constantes.

~~~
package com.usauriorawr.usaurioRAWR_Leccion1VariablesYConstantes`
~~~

~~~
import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
~~~


~~~
class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
    }
}
~~~

~~~
private fun variablesYConstantes() {
~~~

> ### Variables

~~~
    	var myFirstVariable = "Hola mundo :3"
    	var myFirstNumber = 1
    	println(myFirstVariable)
~~~


>Una Variable puede cambiar su valor a lo largo de la ejecucion.

~~~
    	myFirstVariable = "Bienvenmidos a mi Variable"
    	println(myFirstVariable)
    
    	//myFirstVariable = 1
~~~

>  ### Errores;
> 
  		/~~~~~~~~~~~~~~~~~~~\
  +.	|myFirstVariable = 1|
 		 \~~~~~~~~~~~~~~~~~~~/
        -. Error; The integer literal does not conform to the expected type String
        -. trad. direc.> El literal entero no se ajusta al tipo esperado String.
        -. trad> El numero entero no se ajusta al tipo (de variable) esperado String.
        * No podemos asignar un tipo Int a una variable de tipo String
              ** Da error debido a que la variable "myFirstVariable" es de tipo Texto(String)
            y nosotros le estamos introduciondo un valor de tipo numero entero(Int).

> #####¿Cuando hemos definido que tipo de variable es?
            -. Definimos indirectamente el tipo de variable, al escribirla por primera vez.
            -. Kotlin asigna automaticamente el tipo de variable que es, respecto al tipo de
            informacion que le introduciendo por primera vez.

~~~
		var mySecondVariable = "Suscribete!"
		println(mySecondVariable)
~~~

> Podemos cambiar el valor de una bariable respecto al valor de orta.

~~~
   		mySecondVariable = myFirstVariable
   	   println(mySecondVariable)
~~~

~~~
   		myFirstVariable = "¿Ya te has suscrito?"
   		println(myFirstVariable)
~~~


> Constantes

~~~
  		val myFirstConstant = "¿Te ha gustado el tutorial?"
  		println(myFirstConstant)
~~~

> ###Errores;
> 
		/~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\
		|myFirstConstant = "Si te ha gustado, dale LIKE"|
	  	\~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~/
			-. Error; Val cannot be reassigned
			-. trad. direc.> Val no se puede reasignar
  	 	* Una constante no puede modificar su valor

~~~
    	val mySecondConstant = myFirstVariable
    	println(mySecondConstant)
~~~

> Una constante puede obtener el valor de una variable.

`}`



