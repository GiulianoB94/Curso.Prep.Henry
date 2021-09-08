# Homework: Definiciones Teóricas.



## Variables
---
Una variable es un pequeño espacio de memoria que el programador va a reservar y ponerle un nombre, para luego almacenar información dentro de la misma.

¿Como declaramos una variable?

Tenemos tres formas diferentes: 

    * Var : Es la forma tradicional de declarar una variable. (ES5)
    * Let : Es otra forma similar a var, pero se comporta de una manera distinta respecto al nivel de "Scope".(ES6)
    * Const : Es un tipo de variable que, como su nombre lo indica, es "Constante", es decir que su valor se define sólo una vez y no puede volver a cambiarse (Como la fecha de nacimiento de una persona).(ES6)

---
## Strings
---
Se conoce a las "Strings" como "Cadenas de texto". 

    Ejemplo: var color = "amarillo";

Como podemos ver, las strings siempre se definen entre comillas dobles ("amarillo") o simples ('amarillo').

---
## Funciones
---

Las funciones son como los objetos, con la diferencia de que estos pueden llamarse o "invocarse" (callable objects).
Su función principal es calcular, modificar y realizar diferentes acciones sobre las variables.

¿Cómo se aplican?
Las funciones se aplican de las siguientes maneras:

    * function miFuncion () {};
    * var otraFuncion = function () {};
    * var otraMas = () => {}; (A este tipo se lo denomina "Función flecha")

Dentro de las "()" se agrega un "Argumento" y dentro de las "{}" se explaya la operación a realizarse.

Pero que son los "Argumentos"?
Una argumento es una variable que se va a colocar dentro de los paréntesis para poder utilizarla en el proceso.


    Ejemplo: 
    
    var funcion = (color) => {
        alert.('Camiseta de color' + color)
    }

    funcion (Rojo); 
    //Camiseta de color Rojo

Pero ojo, no siempre va a ser sólo una, sino que pueden ser más. Por ejemplo:

    var funcion = (color, talle) => {
        alert.('Camiseta de color ' + color + ' talla ' + talle)
    }

    funcion (Rojo, XL);
    //Camiseta de color Rojo talla XL


En los ejemplos anteriores utilizamos "alert" para mostrar los resultados. En la vida real, vamos a necesitar que la función nos devuelva un valor para poder utilizarlo dentro de la siguiente operación que realizemos. Para ello, utilizamos una palabra llamada "return" (Devolver, en inglés).

¿Y a donde se aplica "return"?

    Ejemplo:
    
     function sumarNum (a, b) {
        var algo = a + b;
        return algo;
    }

    sumarNum (2, 5); // 7

Lo aplicamos cuando ya tengamos todo listo para mostrar en pantalla el resultado que esperamos.

>> Si quisiéramos llamar a la variable "algo" que declaramos en nuestra función, pero por fuera de ella, nos retornaría "undefined" , porque solo pertenece a la función.

---
## Declaraciones ( if )
---

"Si me voy caminando, demoraría 30 minutos. De lo contrario, si me voy en colectivo, demoraría 15."

En este ejemplo vemos que si se realiza una acción, tiene su consecuencia. De lo contrario, tendría otro tipo de consecuencia distinto. Para eso utilizamos la sentencia "if", quiere decir que si un valor es "true" va a suceder algo y la función se dentendrá. De lo contrario (else), si es "false", va a suceder otra cosa y va a omitir la primera parte. 

La sentencia "if" va siempre dentro de una función.

    Ejemplo:

        function idaAlTrabajo (caminando) {
            if (caminando === true) {
                return ("30 minutos de demora")
            } else {
                 return ("15 minutos de demora")
            }
        }; 

---
## Valores Booleanos
---        

Anteriormente vimos las palabras "true" (verdadero) y "false"(falso). En programación, esos valores se denominan "Booleanos" o "Booleans", en inglés. Básicamente son como un botón de encendido/apagado y son los únicos datos booleanos posibles.

    Ejemplo: 

        luzEncendida = true; // La luz está encendida.
        luzEncendida = false; // La luz está apagada.

   