# Programación | P1.1

### PROBLEMA
Haciendo uso de las primitivas que hemos visto aqui. Escribe los algoritmos para solucionar: 
  
1. - Si un número "p" es par o impar.
2. - La tabla del número "p" desde el 1 hasta el 10.
3. - Si un número "p" es primo.

Cada ejercicio en un archivo, almacenado en Repositorio.

### EXPLICACIÓN
1. - Si un número "p" es par o impar.

Procedemos ha analizarlo matemáticamente para saber su lógica e incluso nos podriamos guiar mediante la propia definicion de ser necesario. La definición formal de un numero par es:

![Definicion Formal Par](https://latex.codecogs.com/svg.latex?p%20\in%20\mathbb{N},%20\text{es%20par}%20\iff\%20p%20\bmod%202%20=%200)

Sabiendo esto, de forma didactica podemos decir que:

![Deduccion](https://latex.codecogs.com/svg.latex?p%20\bmod%202%20=%200%20\iff\%202%20\mid%20p)

Entonces lo que hacemos es evaluar mediante una condicional si el resto de p es 0 cuando se divide entre 2, si es verdadera se imprime "Es par", de ser falsa se imprime "Es impar".

2. - La tabla del número "p" desde el 1 hasta el 10.
  
Mediante un bucle desde 1 hasta 10 escribimos la multiplicacion de p * i, siendo i el iterador por cada tabla

3. - Si un número "p" es primo.

Procedemos ha analizarlo matemáticamente para saber su lógica e incluso nos podriamos guiar mediante la propia definicion de ser necesario. La definición formal de un numero par es:

![Definicion Forma Primo](https://latex.codecogs.com/svg.latex?p%20%5Cin%20%5Cmathbb%7BN%7D,%5C;%20p%20%3E%201%20%5C;%5C;%5Ctext%7Bes%20primo%7D%20%5C;%5C;%5Ciff%5C;%5C;%20%5Cforall%20d%20%5Cin%20%5Cmathbb%7BN%7D,%5C;%20%5Cbig(d%20%5Cmid%20p%20%5C;%5CRightarrow%5C;%20(d%20=%201%20%5C;%5Clor%5C;%20d%20=%20p)%5Cbig))

Primo mediante un condicional evaluamos si nuestro numero es menor o igual a 1 para poder descartarlo y solo quedarnos con los Naturales. Despues mediante un bucle desde p-1 porque vamos a íterar desde nuestro minímo sin tomar el propio minímo porque cualquier numero siempre sera divisor de el mismo, hasta máximos el cual como estamos definidos en todos los Naturales, N = {(0), 1, 2, 3...}, lo tomamos hasta el 2, porque en 1 sabemos que siempre sera divisor. Basicamente, nuestro rango es [2, p-1]. Por ultimo, evaluamos por un condicional si el resto es 0 a la hora de dividirlo entre i para saber si es primo, ademas rompemos el bucle para optimizar el proceso, ya que una vez ejecutado nuestro condicional no nos interesa continuar evaluando. Imprimimos a parte usando la variable booleana creada para imprimir nuestro texto y que no se solapen ambos.


