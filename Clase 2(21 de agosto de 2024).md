# Introduccion a la Dinámica de sistemas 
En esta clase definimos conceptos importantes para el desarrollo de la asignatura, cada uno de estos conceptos nos da una acercamiento a la Dinámica de sistemas, tambien empezamos un repaso de algunos temas matematicos que debemos tener en cuenta para mas adelante poder dar solución a los ejercios que realizaremos en la asignatura. 
## 1. Conceptos importantes 
>🔑Sistema: Combinación de componentes que actuan conjuntamente para alcanzar un objetivo
![Sistema](https://github.com/diegavila00/Apuntes/blob/main/TP/sistema.png)
Figura 1. Descripcion grafica de sistema 

>🔑 Sistema Dinamico:Un sistema se llama dinamico si su salida en el presente depende de una entrada en el pasado

>🔑Planta: Toodo lo fisico que permite que sse lleve acabo un proceso

>🔑Proceso: Secuencia de pasos que permite el desarrollo o fabricacion de un objeto o producto.

>🔑Modelos Dinamicos: En control interesa  obtner un modelo matematico que relacione las variables de interes con el tiempo.

>🔑Sistema lineal: Cumple el principio de superpocición y halla proporcionalidad entre entrada y salida.

## 2. Temas para recordar de calculo diferencial  
### 2.1 Derivada  

$lim_{h \to 0}\frac{f(x+h)-f(x)}{h}$


💡Ejemplo 1. 

$f(x)=x^2\longrightarrow \frac{df(x)}{dx}=2x$

### 2.2 Forma general de una ecuaciones diferenciales 
![](https://github.com/diegavila00/Apuntes/blob/main/TP/e.png)

#### 2.2.1 Caracteristicas de una ecuacion diferencial 
##### 2.2.1.1 Ecuacion lineal invariante en el tiempo .

💡Ejemplo 2.

$\frac{d^2x(t)}{dt^2}+8\frac{dx(t)}{dt}+20x(t)=0$

##### 2.2.1.2 Ecuacion lineal variante en el tiempo 

💡Ejemplo 3.

$\frac{d^2x(t)}{dt^2}+(5-sin(2t))x(t)=0$

## 3. Transformada de Laplace 
Es un cambio de espacio geometrico del dominio del tiempo hacia el dominio de la frecuencia compleja.


$X(s)=\int_{0}^{\infty} x(t)  e^{-st} \,dt $

### 3.1 Tranformada inversa de Laplace 
$x(t)=\frac{1}{2\pi j}\int_{c-j\infty }^{c+j\infty} X(s) e^{-st} \,ds$

### 3.2 Principales reglas de tranformada de Laplace 
#### 3.2.1 Tranformada de una funcion 
$L[f(t)]=F(s)$
#### 3.2.2 Tranformada de la derivada 
$L[f'(t)]=sF(s)-f(0)$

$L[f''(t)]=s^2F(s)-sf(0)-f'(0)$

$L[f(t)]=s^nF(s)-s^{n-1}f(0)-.......-sf^{n-1}(0)-f^n(0)$
#### 3.2.3 Tranformada de la integral 
$L\left( \int f(t)dt\right)=\frac{1}{s}F(s)$

### 3.1.3 Algunas de las tranformadas de Laplace que mas usaremos en la asignatura 
#### 3.1.3.1 Trsnformada escalón unitario 
$L[1(t)]=\frac{1}{S}$
#### 3.1.3.2 Tranformada funcion rampa 
$L[A(t)]=\frac{A}{S^2}$
#### 3.1.2.3 Tranformada funcion senosoidal 
$L[Asen\omega t]=\frac{A\omega}{s^2+\omega^2}$
## 4. Calculo de tranformada de Laplace 
Si la funcion lo permite utilizar tablas de trasformadas, si la función es una combinación de varias funciones, expandir en fracciones parciales para obtener suma de funciones que se pueden encuntran en la tabla de tranformadas de Laplace 
### 4.1 Casos de la fracciones parciales 
#### 4.1.1 Caso 1(El denominador tiene raices reales distintos)

$G(S)=\frac{P(s)}{Q(s)}= \frac{P(s)}{(s+p_{1})(s+p_{2})...(s+p_{n})}$

-Sepración en fracciones parciales 

$G(s)=\frac{A}{(s+p_{1})}+\frac{B}{(s+p_{2})}+.....+\frac{N}{(s+p_{n})}$

-A,B.......,N son los coeficinetes que debemos encontrar 

💡Ejemplo 4.
Dterminar la tranformada de la inversa de:

$G(s)=\frac{2s^2-4}{(s+1)(s-2)(s-3)}$

-Solución 


$G(s)=\frac{2s^2-4}{(s+1)(s-2)(s-3)}=\frac{A}{s+1}+\frac{B}{s-2}+\frac{C}{s-3}$

$2s^2-4=A(s-2)(s-3)+B(s+1)(s-3)C(s+1)(s-2)$

$2s^2-4=As^2-5As+6A+Bs^2-2Bs-3B+C^2-Cs-2C$

$$
\begin{align*}
A + B + C &= 2 \\
-5A - 2B - 3C &= 0 \\
6A - 3B + 2C &= -4
\end{align*}
$$

$$
\begin{align*}
A=-\frac{1}{6}\\
B=-\frac{4}{3}\\
C=\frac{7}{2}\\
\end{align*}
$$

$\frac{A}{s+1}+\frac{B}{s-2}+\frac{C}{s-3}= -\frac{1/6}{(s+1)}-\frac{4/4}{(s-2)}+\frac{7/2}{(s-3)}$ 

$L^{-1}=-\frac{1}{6}e^{-t}-e^{2t}+\frac{7}{2}e^{3t}$

## 5. Ejercicios 
📚Ejercico 1. 
Determinar la tranformada inversa de:

$H(s)=\frac{1}{s^2+s+2}$

$\frac{1}{s^2+s+2}=\frac{1}{(s+2)(s-1)}=\frac{A}{s+2}+\frac{B}{s-1}$

$$
\begin{align*}
s=1\\
1=3B\\
\frac{1}{3}=B\\
\end{align*}
$$

$$
\begin{align*}
s=-2\\
1=-3A\\
-\frac{1}{3}=A
\end{align*}
$$

$\frac{A}{s+2}+\frac{B}{s-1}=-\frac{1/3}{s+2}+\frac{1/3}{s-1}$

$L^{-1}=-\frac{1}{3}e^{-2t}+\frac{1}{3}e^{t}$

📚Ejercico 2.
Determinar la tranformada inversa de:
$F(s)=\frac{2s-5}{s^2+36}$

$\frac{2s-5}{s^2+36}=\frac{2s}{^s2+36}-\frac{5}{s^2+36}$

$L^{-1}=2cos(6t)-\frac{5}{6}sen(6t)$

## 6. Conclusion
-Para el desarrollo del curso es demasiado importante tener claro el desarrollo de la transformada de Laplace 





