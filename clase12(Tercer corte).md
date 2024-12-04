# Diagrama de flujo de señales

## 1. ¿Qué es un diagrama de flujo de señalas?
Es una representación gráfica que ilustra cómo se mueven las señales o la información dentro de un sistema, generalmente en el contexto de ingeniería de control, telecomunicaciones o procesamiento de señales. Este tipo de diagrama utiliza bloques, flechas y nodos para mostrar las relaciones funcionales entre las señales de entrada, los procesos intermedios y las salidas.

## 2. Elementos de de los diagrmas de flujo de señales

- Nodos: Representan variables (entradas, salidas o intermedias) dentro del sistema
- Flechas: Indican la dirección del flujo de la señal, es decir, cómo se transfiere o transforma la información de un nodo a otro.
- Bloques funcionales: Representan operaciones matemáticas o lógicas que procesan las señales, como amplificaciones, sumas, integraciones, etc.
- Puntos de suma/resta: Representan combinaciones de señales (suma o resta de múltiples señales).
- Ganancias: Factores que multiplican una señal (representados a menudo como constantes en las flechas).

## 3. Diferencia con diagrama de bloques.
Aunque están relacionados, un diagrama de flujo de señales es más detallado y se enfoca en el movimiento de señales y sus transformaciones matemáticas, mientras que un diagrama de bloques se centra en una visión general de las funciones principales de un sistema.

## 4. Definiciones para tener en cuenta.
- Camino o trayectoria: Es un recorrido de ramas conectadas en el sentido de las flechas de las ramas
- Ganancia de lazo: Es el producto de las ganancias de ramas de un lazo:
- Trayectoria directa: Es el trayecto de in nodo de entrada a un nodo de salida sin cruzar ningún nodo más de una vez.
- Ganancia de trayecto directo: Es el producto de las ganancias de rama de un camino o trayecto directo
- Lazo: Es un camino o trayecto cerrado.
- Ganancia de lazo: Es el producto de las ganancias de ramas de un lazo.

## 5. Fórmula de Mason 

$P=\frac{1}{\bigtriangleup}\sum_{k}P_K\bigtriangleup_K$

- $P_K$ =Ganacia de los caminos directos
- $\bigtriangleup$= 1 − (suma ganancias de los lazos) + (suma producto de 2
lazos que no se tocan) – (suma producto de 3 lazos que no se
tocan)+...
- $\bigtriangleup_K$= 1 −(suma ganancias lazos que no toquen la trayectoria
𝑃𝑘)+(suma ganancias 2 lazos que no toquen la trayectoria 𝑃𝑘 y
no se toquen entre sí)-(suma ganancias 3 lazos que no toquen
la trayectoria 𝑃𝑘 y no se toquen entre sí)+…




























