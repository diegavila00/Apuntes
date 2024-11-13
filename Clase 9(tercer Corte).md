# Función de tranferencia 

## 1. ¿Qué es una función de transferencia(FT)?
Una función de transferencia es la relación entre la salida y la entrada de un sistema, por lo general se expresa de la siguiente manera:
$G(s)=\frac{Y(s)}{U(s)}$

## 2. Casos de una FT
$G(s)=\frac{Y(s)}{U(s)}$

>🔑 Todas las condiciones iniciales de la ecuación son iguales a cero 

>🔑
>n
>$\longrightarrow$
>Polinomio numerador

>🔑
>m
>$\longrightarrow$
>Polonomio denominador
>

n>m Impropia $\rightarrow$ Cambios en la salida sin inyectarle una entrada 

m>n Estrictamente propia $\rightarrow$ Cambios en la salida con una entrada 

n=m Bipropia $\rightarrow$ Instantaneamnete ocurren cambios en la salida cuando se le inyecta una entrada 

💡Ejemplo 1.

$s^2+1\rightarrow$ Impropia.

$2\rightarrow$ Bipropia.

$\frac{1}{s+1}\rightarrow$ Estrictamente propia.

## 2. Ceros de una FT
Para hallar los ceros de una FT debemos igualar a 0 el numerador, despejamos  "s" y los representamos en el plano complejo con un $\bigcirc$

💡Ejemplo 2.
Hallar los ceros de la siguiente FT

$\frac{3s-1}{S^2+3s+2}$

- Igualando el numerador a 0

$3s-1=0$

$s=\frac{1}{3}$

![](https://github.com/diegavila00/Apuntes/blob/main/TP/0.png)

## 3. Polos de un sistema 
Para hallar los polos de un sistema igualamos el denominador a 0, despejamos "s" y los presentamos en el plano complejo con una $\times$

💡Ejemplo 3.

$D(s)=S^2+3s+2$

$(s+1)(s+2)=0$

- $S_1=-1$
- $S_2=-2$

![](https://github.com/diegavila00/Apuntes/blob/main/TP/p.png)

## 3.1 Casos de polos de un sistema 

- Polos reales e iguales

![](https://github.com/diegavila00/Apuntes/blob/main/TP/p1.png)

- Polos reales diferentes
  
![](https://github.com/diegavila00/Apuntes/blob/main/TP/p2.png)

- Polos conjugados

![](https://github.com/diegavila00/Apuntes/blob/main/TP/p3.png)

## 4. Teorema del valor final 

>🔑
>$t=\infty$

- Error en esatdo estacionario.

$\lim_{t\to\infty} f(t)=\lim_{s\to 0}sF(s)$

💡Ejemplo 4.

$G(s)=\frac{Y(s)}{U(s)}=\frac{4}{5s+1}\rightarrow Y(s)=\frac{4}{5s+1}U(s)$

>🔑U(s)=escalon
>$\rightarrow \frac{1}{s}$

$Y(s)=\frac{4}{5s+1}\frac{1}{s}$

$\lim_{s\to 0}S\left(\frac{4}{5s+1}\right)\left(\frac{1}{s}\right)\rightarrow \lim_{s\to}\frac{4}{5(0)+1}\rightarrow 4$

## 5. Ejercicos 

📚 Ejercico 1.

Realizar el mapa de polos y ceros para el siguiente sistema.
$\frac{s+5}{s^2+5s+6}$

- Ceros

$s+5=0$

$s=-5$

- Polos

$s^2+5s+6=0$

$s_1=-3$

$s_2=-2$

![](https://github.com/diegavila00/Apuntes/blob/main/TP/m1.png)

📚 Ejercico 2.

Realizar el mapa de polos y ceros para el siguiente sistema.
$\frac{3s+4}{3s^3+s^2+9s+2}$

- Ceros

$3s+4=0$

$s=-\frac{4}{3}$

- Polos

$3s^3+s^2+9s+2=0$

$s_1=-0.22$

$s_2=-0.054+1.74$

$s_3=-0.054-1.74$

![]()


