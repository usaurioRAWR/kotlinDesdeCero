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
![Run(1) - Lección_1](https://github.com/usaurioRAWR/kotlinDesdeCero/blob/97f115b228da9cd0cf1a78e3d163de57bf84d7f9/Lecci%C3%B3n%201%20-%20Variables%20y%20constantes./000%20-%20Imagenes/:*Run(1)*:%20Lecci%C3%B3n_1_-_Variables_y_constantes._(_usaurioRAWR!_)_app%20.png)

>Una Variable puede cambiar su valor a lo largo de la ejecucion.

~~~
	myFirstVariable = "Bienvenmidos a mi Variable"
    	println(myFirstVariable)
~~~
![Run(2) - Lección_1](https://github.com/usaurioRAWR/kotlinDesdeCero/blob/97f115b228da9cd0cf1a78e3d163de57bf84d7f9/Lecci%C3%B3n%201%20-%20Variables%20y%20constantes./000%20-%20Imagenes/:*Run(2)*:%20Lecci%C3%B3n_1_-_Variables_y_constantes._(_usaurioRAWR!_)_app%20.png)
~~~
    	//myFirstVariable = 1
~~~


>  #### Errores;
> 
> 		/~~~~~~~~~~~~~~~~~~~\
>		|myFirstVariable = 1|
>		\~~~~~~~~~~~~~~~~~~~/
>			-. Error; The integer literal does not conform to the expected type String
>			-. trad. direc.> El literal entero no se ajusta al tipo esperado String.
>			-. trad> El numero entero no se ajusta al tipo (de variable) esperado String.
>			* No podemos asignar un tipo Int a una variable de tipo String
> 			** Da error debido a que la variable "myFirstVariable" es de tipo Texto(String)
>			y nosotros le estamos introduciondo un valor de tipo numero entero(Int).
>
> #### ¿Cuando hemos definido que tipo de variable es?
>            -. Definimos indirectamente el tipo de variable, al escribirla por primera vez.
>            -. Kotlin asigna automaticamente el tipo de variable que es, respecto al tipo de
>            informacion que le introduciendo por primera vez.

~~~
	var mySecondVariable = "Suscribete!"
	println(mySecondVariable)
~~~

![Run(3) - Lección_1](https://github.com/usaurioRAWR/kotlinDesdeCero/blob/97f115b228da9cd0cf1a78e3d163de57bf84d7f9/Lecci%C3%B3n%201%20-%20Variables%20y%20constantes./000%20-%20Imagenes/:*Run(3)*:%20Lecci%C3%B3n_1_-_Variables_y_constantes._(_usaurioRAWR!_)_app.png)

> Podemos cambiar el valor de una bariable respecto al valor de orta.

~~~
	mySecondVariable = myFirstVariable
	println(mySecondVariable)
~~~

![Run(4) - Lección_1](https://github.com/usaurioRAWR/kotlinDesdeCero/blob/97f115b228da9cd0cf1a78e3d163de57bf84d7f9/Lecci%C3%B3n%201%20-%20Variables%20y%20constantes./000%20-%20Imagenes/:*Run(4)*:%20Lecci%C3%B3n_1_-_Variables_y_constantes._(_usaurioRAWR!_)_app%20.png)

~~~
	myFirstVariable = "¿Ya te has suscrito?"
	println(myFirstVariable)
~~~

![Run(5) - Lección_1](https://github.com/usaurioRAWR/kotlinDesdeCero/blob/97f115b228da9cd0cf1a78e3d163de57bf84d7f9/Lecci%C3%B3n%201%20-%20Variables%20y%20constantes./000%20-%20Imagenes/:*Run(5)*:%20Lecci%C3%B3n_1_-_Variables_y_constantes._(_usaurioRAWR!_)_app%20.png)

> Constantes

~~~
	val myFirstConstant = "¿Te ha gustado el tutorial?"
	println(myFirstConstant)
~~~

![Run(6) - Lección_1](https://github.com/usaurioRAWR/kotlinDesdeCero/blob/97f115b228da9cd0cf1a78e3d163de57bf84d7f9/Lecci%C3%B3n%201%20-%20Variables%20y%20constantes./000%20-%20Imagenes/:*Run(6)*:%20Lecci%C3%B3n_1_-_Variables_y_constantes._(_usaurioRAWR!_)_app%20.png)

> ###Errores;
> 
>		/~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\
>		|myFirstConstant = "Si te ha gustado, dale LIKE"|
>		\~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~/
>			-. Error; Val cannot be reassigned
>			-. trad. direc.> Val no se puede reasignar
>  	 		* Una constante no puede modificar su valor

> Una constante puede obtener el valor de una variable.

~~~
    	val mySecondConstant = myFirstVariable
    	println(mySecondConstant)
~~~

![Run(7) - Lección_1](https://github.com/usaurioRAWR/kotlinDesdeCero/blob/97f115b228da9cd0cf1a78e3d163de57bf84d7f9/Lecci%C3%B3n%201%20-%20Variables%20y%20constantes./000%20-%20Imagenes/:*Run(7)*:%20Lecci%C3%B3n_1_-_Variables_y_constantes._(_usaurioRAWR!_)_app%20.png)

`}`



