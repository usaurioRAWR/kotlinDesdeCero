	// <Inicio> Aqui vamos a hablar de variables y constantes.--------------------------------------
    private fun variablesYConstantes() {
        // <Inicio> Variables-----------------------------------------------------------------------
            var myFirstVariable = "Hola mundo :3"
            var myFirstNumber = 1
            println(myFirstVariable)

            // Una Variable puede cambiar su valor a lo largo de la ejecucion.
            myFirstVariable = "Bienvenmidos a mi Variable"
            println(myFirstVariable)

            /*
                +. myFirstVariable = 1
                    -. Error; The integer literal does not conform to the expected type String
                    -. trad. direc.> El literal entero no se ajusta al tipo esperado String.
                    -. trad> El numero entero no se ajusta al tipo (de variable) esperado String.

                    * No podemos asignar un tipo Int a una variable de tipo String

                    ** Da error debido a que la variable "myFirstVariable" es de tipo Texto(String)
        y nosotros le estamos introduciondo un valor de tipo numero entero(Int).

                +. ¿Cuando hemos definido que tipo de variable es?
                    -. Definimos indirectamente el tipo de variable, al escribirla por primera vez.
                    -. Kotlin asigna automaticamente el tipo de variable que es, respecto al tipo de
        informacion que le introduciendo por primera vez.
            */
            var mySecondVariable = "Suscribete!"
            println(mySecondVariable)

            mySecondVariable = myFirstVariable
            println(mySecondVariable)

            myFirstVariable = "¿Ya te has suscrito?"
            println(myFirstVariable)
        // <Fin> Variables--------------------------------------------------------------------------
        // <Inicio> Constantes----------------------------------------------------------------------
            val myFirstConstant = "¿Te ha gustado el tutorial?"
            println(myFirstConstant)
            /*
                myFirstConstant = "Si te ha gustado, dale LIKE"
                    Error; Val cannot be reassigned
                        trad. direc.> Val no se puede reasignar

                * Una constante no puede modificar su valor
             */
            // Una constante puede obtener el valor de una variable.
                val mySecondConstant = myFirstVariable
                println(mySecondConstant)
        // <Fin> Constantes-------------------------------------------------------------------------
    }
    // <Fin> Aqui terminamos de hablar de variables y constantes.-----------------------------------
