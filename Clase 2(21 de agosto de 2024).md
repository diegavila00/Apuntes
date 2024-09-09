# Introduccion a la Dinámica de sistemas 
En esta clase definimos conceptos importantes para el desarrollo de la asignatura, cada uno de estos conceptos nos da una acercamiento a la Dinámica de sistemas, tambien empezamos un repaso de algunos temas matematicos que debemos tener en cuenta para mas adelante poder dar solución a los ejercios que realizaremos en la asignatura. 
## 2. Conceptos importantes 
>🔑Sistema: Combinación de componentes que actuan conjuntamente para alcanzar un objetivo
![Sistema](https://github.com/diegavila00/Apuntes/blob/main/TP/sistema.png)
Figura 1. Descripcion grafica de sistema 

>🔑 Sistema Dinamico:Un sistema se llama dinamico si su salida en el presente depende de una entrada en el pasado

>🔑Planta: Toodo lo fisico que permite que sse lleve acabo un proceso

>🔑Proceso: Secuencia de pasos que permite el desarrollo o fabricacion de un objeto o producto.

>🔑Modelos Dinamicos: En control interesa  obtner un modelo matematico que relacione las variables de interes con el tiempo.

>🔑Sistema lineal: Cumple el principio de superpocición y halla proporcionalidad entre entrada y salida.

## 3. Temas para recordar de calculo diferencial  
### 3.1 Derivada  

$lim_{h \to 0}\frac{f(x+h)-f(x)}{h}$


💡Ejemplo 1. 

$f(x)=x^2\longrightarrow \frac{df(x)}{dx}=2x$

### 3.2 Forma general de una ecuaciones diferenciales 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/e.png)

#### 3.2.1 Caracteristicas de una ecuacion diferencial 
##### 3.2.1.1 Ecuacion lineal invariante en el tiempo .

💡Ejemplo 2.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/Captura%20de%20pantalla%202024-09-06%20181925.png)

##### 3.2.1.2 Ecuacion lineal variante en el tiempo 

💡Ejemplo 3.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/Captura%20de%20pantalla%202024-09-06%20182427.png)


## 4. Transformada de Laplace 
Es un cambio de espacio geometrico del dominio del tiempo hacia el dominio de la frecuencia compleja.

![Formula transformada de Laplace](https://github.com/diegavila00/Apuntes/blob/main/TP/P.png)

### 4.1 Tranformada inversa de Laplace 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/Captura%20de%20pantalla%202024-09-06%20183058.png)

### 4.2 Principales reglas de tranformada de Laplace 
#### 4.2.1 Tranformada de una funcion 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/L%20funcion.png)
#### 4.2.2 Tranformada de la derivada 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/L%20derivada.png)
#### 4.2.3 Tranformada de la integral 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/L%20integral.png)

### 4.1.3 Algunas de las tranformadas de Laplace que mas usaremos en la asignatura 
#### 4.1.3.1 Trsnformada escalón unitario 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/escalon.png)
#### 4.1.3.2 Tranformada funcion rampa 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/Captura%20de%20pantalla%202024-09-09%20100859.png)
#### 4.1.2.3 Tranformada funcion senosoidal 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/seno.png)
## 5. Calculo de tranformada de Laplace 
Si la funcion lo permite utilizar tablas de trasformadas, si la función es una combinación de varias funciones, expandir en fracciones parciales para obtener suma de funciones que se pueden encuntran en la tabla de tranformadas de Laplace 
### 5.1 Casos de la fracciones parciales 
#### 5.1.1 Caso 1(El denominador tiene raices reales distintos)

![](https://github.com/diegavila00/Apuntes/blob/main/TP/fp.png)

-Sepración en fracciones parciales 

![](https://github.com/diegavila00/Apuntes/blob/main/TP/dFP.png)

-A,B.......,N son los coeficinetes que debemos encontrar 

💡Ejemplo 4.
Dterminar la tranformada de la inversa de:

![](https://github.com/diegavila00/Apuntes/blob/main/TP/ejemplo%20caso%201.png)

-Solución 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/Solucion%20ejemplo%20caso%201.png)

$G(s)=\frac{2s^2-4}{(s+1)(s-2)(s-3)}=\frac{A}{s+1}+\frac{B}{s-2}+\frac{C}{s-3}$

$x(t)=2x$







