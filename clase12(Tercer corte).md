# Diagrama de flujo de señales(Diego Avila y Santigo Garcia)
En esta clase vimos que es un diagrama de flujo de señales, que elementos lo componen, definicones muy importantes que se deben tener en cuenta para el analisis y el desarrollo de este tipo de diagramas usando la formula de Mason. 
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

💡Ejemplo 1.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/fm.png)

- Trayectorias directas

$P_1= G_1* G_2* G_3$

- Lazos cerrados

$L_1=G_1* G_2* H_1$

$L_2= -G_2 * G_3 * H_2$

$L_3= -G_1 * G_2 * G_3$

- $\bigtriangleup= 1-(L_1+L_2+L_3)$

- $\bigtriangleup_1=1$

$\frac{C(s)}{R(s)}=\frac{P_1\bigtriangleup_1}{\bigtriangleup}=\frac{G_1* G_2* G_3}{1-G_1* G_2* H_1+G_2 * G_3 * H_2+G_1 * G_2 * G_3}$


## 6. Ejercicios 

📚 Ejercico 1.

Usando la formula de Mason desarrolar lo siguiente.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/df1.png)

- Desarrollo

$P_1=G1* G2* G3* G4* G5$

$P_2=G1 * G6 * G4 * G5$

$P_3=G1 * G2* G7$

$L_1= -G4 *H1$

$L_2= -G2 *G7 *H2$

$L_3= -G6 * G4 * G5 * H2$

$L_4= -G2 * G3 * G4 * G5 * H2$

- $\bigtriangleup=1-(L1+L2+L3+L4)+L1*L2$
- $\bigtriangleup_1=1$
- $\bigtriangleup_2=1-L1$

$P=\frac{G1* G2* G3* G4* G5+G1 * G6 * G4 * G5(1+G4H1)}{1+G4 *H1+G2 *G7 *H2+G6 * G4 * G5 * H2+G2 * G3 * G4 * G5 * H2+ G4 *H1 *G2 *G7 *H2}$

📚 Ejercico 2. 


## 7. Concluiones 

- Los diagramas de flujo de señales son herramientas fundamentales para analizar y entender el comportamiento de sistemas dinámicos complejos. Permiten desglosar un sistema en sus elementos básicos (entradas, procesos y salidas) y estudiar cómo interactúan entre sí, facilitando su modelado y análisis matemático.
-  La fórmula de ganancia de Mason proporciona un método sistemático para calcular la relación entre la salida y la entrada de un sistema complejo. Esto permite analizar sistemas con múltiples trayectorias, lazos y relaciones interdependientes de forma eficiente y ordenada.
  
## 8. Referencias 

- Esquivel, A. [@aurelianoesquivel]. (s/f). Lección 28 Fórmula de Mason y los diagramas de flujo de señales, y un ejemplo. Youtube. Recuperado el 5 de diciembre de 2024, de https://www.youtube.com/watch?v=bFs_jfXCdLg
- (S/f). Recuperado el 5 de diciembre de 2024, de http://chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://virtual.usalesiana.edu.bo/web/contenido/dossier/22011/698.pdf



























