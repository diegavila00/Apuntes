# Diagramas de bloques
En esta clase hablamos sobre los diagramas de bloques y álgebra de bloques,un diagrama de bloques es una forma fácil y visual de entender cómo funciona un sistema, mostrando sus partes principales y cómo las señales pasan de una a otra. Los bloques representan procesos, las flechas indican el flujo, y elementos como los puntos de suma o las ramificaciones ayudan a combinar o dividir señales.
## 1. Definición
Es la representación del funcionamiento interno de un sistema, que se hace mediante bloques y sus relaciones, y que, además, definen la organización de todo el proceso interno, sus entradas y sus salidas.

## 2. Elementos de un diagrama de bloques

- Bloque Funcional.

Representa la operación matemática sobre la señal de entrada para generar la salida.
![](https://github.com/diegavila00/Apuntes/blob/main/TP/pp.png)

- Flechas.

Representan las señales dentro del proceso. La punta de la flcha que señala el bloque indica la entrada y la punta de flecha que se aleja del bloque representa la salida. 


![](https://github.com/diegavila00/Apuntes/blob/main/TP/FF.png)

- Punto suma.

Realiza operaciones ya sea suma o resta unicamente entre señales, el signo en cada punta de flecha indica si la señal debe sumarse o restarse.

>🔑 Las cantidades que se sumen o resten deben tener las mismas dimensiones y las mismas unidades.


![](https://github.com/diegavila00/Apuntes/blob/main/TP/sss.png)

- Ramificación

Un punto de ramificacion es el punto en el que la señal de un bloque va de forma simultánea a otros bloques o puntos sumas.
![](https://github.com/diegavila00/Apuntes/blob/main/TP/rrr.png)

- Interpretación del diagrama de bloques.


La salida del bloque funcional es la multiplicación de la entrada por la función de transferencia del bloque.

$Y(s)=U(s)*G(s)$

![](https://github.com/diegavila00/Apuntes/blob/main/TP/pp2.png)

💡Ejemplo 1.

Identifique los elementos del siguiente sistema.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/%C3%B1.png)

- Flechas
- Punto suma
- Bloque Funcional
- Ramificación 

## 3. Álgebra de bloques 
Es un conjunto de reglas que permiten transformar los diagrama de bloques, similar al álgebra que permite transformar las ecuaciones lineales.
Algunas de esas reglas son:

![](https://github.com/diegavila00/Apuntes/blob/main/TP/reglas.png)

💡Ejemplo 2.

Reducir el siguiente diagrama de bloques.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/wwww.png)

>🔑
>Usamos esta regla
>![](https://github.com/diegavila00/Apuntes/blob/main/TP/oooooooooo.png)

- Diagrama de bloques resultante.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/xxxxxx.png)


💡Ejemplo 3.

Reducir el siguiente diagrama de bloques.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/bbbbbb.png)

- Procedimiento

![](https://github.com/diegavila00/Apuntes/blob/main/TP/aaaaaaaa.png)

![](https://github.com/diegavila00/Apuntes/blob/main/TP/nnnnnnnn.png)

![](https://github.com/diegavila00/Apuntes/blob/main/TP/cccccc.png)

![](https://github.com/diegavila00/Apuntes/blob/main/TP/RRRRRR.png)

## 4. Ejerccios 

📚 Ejercico 1. 

Realice la reducción usando álgebra de bloques.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/eje1.png)

- Procedimiento 

![]()

## 5. Cunclusiones 

- Los diagramas de bloques permiten representar visualmente procesos complicados, haciendo más sencillo identificar cómo funcionan y cómo interactúan sus componentes principales.
- Ayudan a analizar, simplificar y optimizar sistemas mediante reglas específicas, lo que es especialmente útil en áreas como la ingeniería y el control de procesos.









