Aproximación de Taylor
Introducción a Brook Taylor
Brook Taylor fue un matemático inglés conocido por sus contribuciones significativas al cálculo diferencial e integral. Su mayor legado es la serie de Taylor, una herramienta poderosa para aproximar valores de una función compleja utilizando valores cercanos de la función y sus derivadas en otro punto.

¿Qué es la Serie de Taylor?
La serie de Taylor permite aproximar el valor de una función 
f
 en un punto 
x
i
+
1
 utilizando la función y sus derivadas en otro punto 
x
i
. La fórmula general es:

f
(
x
i
+
1
)
=
f
(
x
i
)
+
f
′
(
x
i
)
1
!
1
(
x
i
+
1
−
x
i
)
+
⋯
+
f
n
(
x
i
)
1
n
!
(
x
i
+
1
−
x
i
)
n
Entendiendo la Serie de Taylor
La serie de Taylor se maneja mediante iteraciones. A más iteraciones, más elementos de la serie se utilizan, lo que mejora la precisión de la aproximación.

Valor Aproximado
El valor aproximado se obtiene utilizando la n-ésima iteración de la serie de Taylor. Por ejemplo, para la primera iteración:

f
(
x
i
+
1
)
=
f
(
x
i
)
+
f
′
(
x
i
)
(
x
i
+
1
−
x
i
)
A más iteraciones, la aproximación será más precisa.

Error del Resultado
El error en la aproximación es el último término de la serie de Taylor utilizado. Por ejemplo, si se hace una sola iteración, el error será:

ϵ
=
∣
f
′
(
x
i
)
(
x
i
+
1
−
x
i
)
∣
Vocabulario Clave
Truncar: Aproximar o cortar valores, convertir un proceso infinito en finito.

Convergencia: Llegar a una solución mediante una función.

Criterio de parada: Condición para terminar las iteraciones, relacionada con la tolerancia.

Ejemplo y Ejercicio
Ejemplo 1: Si tenemos el número 123.123, para convertirlo a la forma descrita:

Desplazamos el número: \[ 123.123 \rightarrow 0.123123 \]

Multiplicamos por la base: \[ 0.123123 \times 10 \]

Elevamos a la cantidad de posiciones desplazadas: \[ 0.123123 \times 10^3 \]

Ejercicio: Comenzando con el error de la máquina (
ϵ
=
2.22
×
1
0
−
16
):

Para equipos de 32 bits:

7 bits para el exponente

23 bits para la mantiza

Valores representativos:

Valor más pequeño: \[ 0.1 \times 2^{-1111111} = 0.5 \times 2^{-256} = 4.3180842775472223 \times 2^{-78} \]

Valor más grande: \[ 0.11...1 \times 2^{111...1} = 0.9999997615814209 \times 2^{4194304} \]

Para equipos de 64 bits:

11 bits para el exponente

52 bits para la mantiza

Valores representativos:

Valor más pequeño: \[ 0.1 \times 2^{-11111111111} = 0.5 \times 2^{-...} \]

Conclusión
La serie de Taylor es una herramienta crucial para la aproximación de funciones complejas en términos de sus derivadas, mejorando la precisión con cada iteración y proporcionando una forma de medir el error.
