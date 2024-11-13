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













