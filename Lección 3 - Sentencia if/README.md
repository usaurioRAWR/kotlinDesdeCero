package com.usauriorawr.usaurioRAWR_Leccion3SentenciaIF

import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle

class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
    }
}
// :-----------------------------------------------------------------------------------------------:
// <Inicio> Aqui vamos a hablar de la sentenci IF.--------------------------------------------------
// :-----------------------------------------------------------------------------------------------:

private fun sentenciaIF() {
    var myNumber = 20
/*:-------------------------------------------------------------------------------------------------
        Operadores condicionales
            > mayor que
            < menor que
            >= mayor o igual que
            <= menor o igual que
            == igualdad
            != desigualdad

        Operadores logicos
            && operador AND (multiplicacion)
            || operador OR (suma)
            ! operador NOT (negacion)
-------------------------------------------------------------------------------------------------:*/

    // Sentencia IF
    if (myNumber < 20 && myNumber > 10) {
        println("$myNumber es menor que 20 y mayor que 10")
    }
    // Sentencia ELSE
    else {
        println("$myNumber es meyor que 20 o menor o igual que 10")
    }
}
// :-----------------------------------------------------------------------------------------------:
// <Fin> Aqui terminamos de hablar de la sentenci IF.-----------------------------------------------------
// :-----------------------------------------------------------------------------------------------:

