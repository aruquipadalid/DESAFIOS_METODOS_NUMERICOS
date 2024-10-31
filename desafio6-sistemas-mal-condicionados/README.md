# SISTEMAS MAL CONDICIONADOS

Un sistema mal condicionado es aquel en el que pequeñas variaciones en los datos de entrada pueden causar grandes cambios en los resultados. Esto puede hacer que los resultados sean poco fiables. Aquí te dejo algunos métodos para detectar si un sistema está mal condicionado:

## Métodos para Detectar Sistemas Mal Condicionados

1. **Número de Condicionamiento**:
   Calcula el número de condicionamiento de la matriz de coeficientes. Si este número es muy grande, el sistema está mal condicionado. El número de condicionamiento se puede calcular como el producto de la norma de la matriz y la norma de su inversa.

   \[
   \text{cond}(A) = \|A\| \cdot \|A^{-1}\|
   \]

2. **Sensibilidad a Perturbaciones**:
   Introduce pequeñas perturbaciones en los coeficientes de la matriz y observa cómo cambian las soluciones. Si las soluciones cambian significativamente, el sistema es mal condicionado.

3. **Normas de Vectores y Matrices**:
   Utiliza normas para medir la magnitud de los vectores y matrices. Las normas más comunes son la norma 1, la norma infinito y la norma euclidiana.

4. **Análisis Gráfico**:
   En algunos casos, puedes representar gráficamente las ecuaciones del sistema. Si las líneas o planos están casi paralelos, el sistema puede estar mal condicionado.

Estos métodos te ayudarán a identificar y manejar sistemas mal condicionados. Si necesitas más detalles, te recomiendo revisar recursos adicionales como videos educativos y artículos especializados.

## Ejemplo de un Sistema Bien Condicionado

```matlab
% Ejemplo 1
a1 = [10 2 -1; -3 -6 2; 1 1 5];
b1 = [27; -61.5; -21.5];
x = inv(a1) * b1;
disp(x); % Resultado: [0.5, 8, -6]
disp(cond(a1)); % Resultado: 2.4580

% A pesar de pequeños cambios, no cambia radicalmente la solución
a1 = [10 1.98 -1; -3 -6 2; 1 1 5];
x = inv(a1) * b1;
disp(x); % Resultado: [0.5177, 7.9906, -6.0017]

# Sistemas Mal Condicionados en Álgebra Lineal

Este repositorio contiene un ejemplo de sistemas de ecuaciones mal condicionados, incluyendo el uso de matrices de Hilbert en Octave.

## Contenido

- **sistemas_mal_condicionados.m**: Este archivo Octave incluye:
  - Un sistema mal condicionado de 2x2, con su número de condición y su gráfica.
  - Una matriz de Hilbert de dimensión 3x3, con su número de condición.

## Instrucciones

Para ejecutar el archivo en Octave:

```octave
sistemas_mal_condicionados

