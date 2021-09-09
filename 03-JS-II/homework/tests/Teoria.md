# Homework: Definiciones Teóricas.

## Bucle 'For'
---

El bucle 'for' posee una estructura similar a 'if', con la particularidad de que es un poco mas complejo.

Dentro de los paréntesis, el desarrollador deberá especificar tres parámetros:


* for ( let i = 0 ;) --> Declarar una variable "i" con su valor inicial.

* ( i > 10 ;) --> La expresión condicional, que indica si la variable debe incrementar, decrementar, etc.

* ( i++ ) --> Esta expresión indica que por cada iteración, el valor de i deberá modificar a su valor actual mas 1.


El resultado final sería algo como esto:


         for (let i = 0; i > 10; i++) {}

El bucle 'for' evaluará si la expresión condiciónal es 'true' o 'false'. En caso de que sea 'true' el bucle volverá a ejecutarse, de lo contario se dentendrá.


---
## Operadores Lógicos

>> &&

El significado de este operador es "Y" (And, en inglés) y como su nombre lo indica, se encarga de cumplir dos (o más) premisas dentro del argumento de una sentencia 'if', por ejemplo.


* Si ambas premisas son verdaderas, devolverá 'true'.
* Si una o ambas premisas son falsas, devolverá 'false'.

        if (100 > 10 && 10 === 10) {
            console.log('Ambas declaraciones son ciertas, este código se ejecutará');
        }


>> ||

Lo mismo sucede con este operador, cuyo significado es 'o' condicional en español (Or, en inglés). La diferencia respecto a && es que:

* Si al menos una premisa es verdadera, devolverá 'true'.
* Si ambas premisas son falsas, devolverá 'false'.

*        if (100 > 10 || 10 === 10) {
            console.log('Ambas declaraciones son ciertas, este código se ejecutará');
        }


*        if (10 === 9 || 10 > 9) {
            console.log('Una de las declaraciones es true, por lo que || devolverá true y este código se ejecutará');
        }


*       if (10 === 9 || 1 > 9) {
            console.log('Ambas declaraciones son falsas, por lo que || devolverá false y este código no se ejecutará');
        }



>>!

El valor 'No' (Not, en inglés) se encargará de devolver el valor opuesto al boolean obtenido, por ejemplo:

*        if (!false) {
            console.log('El ! devolverá true, porque es lo contrario de false, así que ste código se ejecutará');
        }

*        if (!(1 === 1)) {
            console.log('1 es igual a 1, de modo que la expresión devuelve true. El operador ! devolverá lo contrario de eso, por lo que este código NO se *ejecutará');
}       