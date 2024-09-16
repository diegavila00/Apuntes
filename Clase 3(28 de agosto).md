# Ecuaciones Diferenciales y metodo resumido de tranformda de Laplace 
Antes de empezar con la solucion de ecuaciones diferenciales y el metodo resumido para la solución de tranformada de Laplace, terminados de repasar los dos casos de descomposición en fracciones parciales que faltaron de la clase anterior los cuales son cuando el Tiene raices reales reptidas y cuando las raices son complejas, tambien aprendimos como solucionar fraciones parciales, la transformada y la transformada inversa de Lplace, ecuaciones diferenciales usando matlab.

## 1. Caso 2 fraciones parciales(n raices reales repetidas)
$G(s)=\frac{P(s)}{Q(s)}=\frac{P(s)}{(s+p)^n}$
- 
-Descomposición en fracciones parciales 

$G(s)=\frac{A}{(s+p)}+\frac{B}{(s+p)}+......+\frac{N}{(s+p)^n}$

💡Ejemplo 1. 

$$G(s)=\frac{2s^2+6s+5}{(s+2)(s+1)}=\frac{A}{S+2}+\frac{B}{s+1}+\frac{C}{(s+1)^2}$$


$2s^2+6s+5=A(s+1)^2+B(s+2)(s+1)+C(s+2)$

$2s^2+6s+5=A^2+2As+A+Bs^2+3Bs+2B+Cs+2C$

-Ecuaciones 

$$
\begin{align*}
2=A+B \\\
6=2A+3B+C\\
5=A+2B+2C\\
\end{align*}
$$

-Coeficientes 

$$
\begin{align*}
A=1 \\\
B=1\\
C=1\\
\end{align*}
$$


$L^{-1}\left(\frac{1}{S+2}+\frac{1}{s+1}+\frac{1}{(s+1)^2}\right)$

-Solución aplicando transformada inversa de Laplace 

$L^{-1}=\left(e^{-2t}+e^{-t}+te^{-t}\right)$
-

## 2. Caso 3(Raices Complejas)
$G\left(s\right)=\frac{P\left(s\right)}{Q\left(s\right)}=\frac{P\left(s\right)}{\left(s^2+b_1s+C_1\right)\left(s^2+b_2s+C_2\right)...\left(s^2+b_ns+C_n\right)}$
-

-Descomposición en fracciones parciales 

$G\left(s\right)=\frac{As+B}{\left(s^2+b_1s+c_1\right)}+\frac{Cs+D}{\left(s^2+b_2s+c_2\right)}+...+\frac{Ms+N}{\left(s^2+b_ns+c_n\right)}$


A, B,C,D,..., M, N son coeficientes por determinar.

💡 Ejermplo 2.

$$G\left(s\right)=\frac{s^2+2s+3}{\left(s^2+2s+2\right)\left(s^2+2s+5\right)}$$

$\frac{s^2+2s+3}{\left(s^2+2s+2\right)\left(s^2+2s+5\right)}=\frac{As+B}{\left(s^2+2s+2\right)}+\frac{Cs+D}{\left(s^2+2s+5\right)}$

$s^2+2s+3=\left(As+B\right)\left(s^2+2s+5\right)+\left(Cs+D\right)\left(s^2+2s+2\right)$

$s^2+2s+3=As^3+2As^2+5As+s^2B+2Bs+5B+s^3C+2s^2C+2Cs+s^2D+2Ds+2D$

-Ecuaciones 

$$
\begin{align*}
0= A + C & \\
1= 2A + B + 2C + D & \\
2= 5A + 2B + 2C +2D & \\
3= 5B + 2D &
\end{align*}
$$

-Coeficientes 

A=0

$\frac{1}{3}$

C=0

$D=\frac{2}{3}$

$\frac{1}{3}\frac{1}{\left(s^2+2s+2\right)}+\frac{2}{3}\frac{1}{\left(s^2+2s+5\right)}$

-Solución aplicando transformada inversa de Laplace 

$𝓛^1\left(\frac{1}{3}\frac{1}{\left(s^2+2s+2\right)}+\frac{2}{3}\frac{1}{\left(s^2+2s+5\right)}\right)$

$$\frac{1}{3}e^{-t}\sin \left(t\right)+\frac{e^{-t}\sin \left(2t\right)}{3}$$
-

## 3. Tranformada inversa (Metodo resumido)

En vista de que las raíces del polinomio del numerador deben factorizarse para descomponer en fracciones parciales, se puede determinar que algunos términos se eliminan en los valores de s. el sistema de ecuaciones que debe ser solucionado se reduce.

$$F(s)=\frac{A(s)}{B(s)}=\frac{a_{1}}{s+p_{1}}+\frac{a_{2}}{s+p_{2}}+......+\frac{a_{n}}{s+p_{n}}$$

Sabiendo que 𝑎𝑘 (𝑘 = 1, 2, 3, … ) son constantes , 𝑎𝑘 puede hallarse multiplicando ambos lados de la igualdad por (𝑠 + 𝑝𝑘 ) y haciendo 𝑠 = −𝑝𝑘 , de lo cual se obtiene

$$\left[(s+p_{k})\frac{A(s)}{B(s)}\right]_{s=-pk} =\left[\frac{a1}{s+p1}(s+pk)+\frac{a2}{s+p2}(s+pk)+.....+\frac{an}{s+pn}(s+pk)\right]=ak$$

$$ a_{k}=\left[(s+p)\frac{A(s)}{B(s)}\right]_{s=-pk} $$

💡 Ejermplo 3.

$$G\left(s\right)=\frac{s+3}{\left(s+1\right)\left(s+2\right)}=\frac{A}{\left(s+1\right)}+\frac{B}{\left(s+2\right)}$$

$\left(s+1\right)\left(\frac{s+3}{\left(s+1\right)\left(s+2\right)}\right)_{s=-1}=\rightarrow$

$\left(s+1\right)\left(\frac{A}{\left(s+1\right)}\right)_{s=-1} + \rightarrow$

$\left(s+1\right)\left(\frac{B}{\left(s+2\right)}\right)_{s=-1}$

2=A

$\left(s+2\right)\left(\frac{s+3}{\left(s+1\right)\left(s+2\right)}\right)_{s=-2}=\rightarrow$

$\left(s+2\right)\left(\frac{A}{\left(s+1\right)}\right)_{s=-2}+\rightarrow $ 

$+\left(s+2\right)\left(\frac{B}{\left(s+2\right)}\right)_{s=-2}$

-1=B

-Solución 

$L^{-1}\left[\frac{2}{s+1}-\frac{1}{s+2}\right]=se^{-t}-e^{-2t}$

## 4. Fracciones parciales en MatLab 
Con el conocimiento de los polinomios del numerador y denominador de la función en el dominio s, Matlab puede calcular los términos de las fracciones parciales.

$$F(s)=\frac{s^2-s-3}{s(s-1)(s+3)}=\frac{0.75}{s-3}-\frac{0.75}{s+1}+\frac{1}{s}$$

-r= Términos del numerador

-p= Términos del denominador

-k= Términos independientes

-Codigo

```
num=[1 -1 -3];
den=conv([1 -1 0],[1 3]);
[r,p,k]=residue(num,den)

r =

    0.7500
   -0.7500
    1.0000
p =

   -3.0000
    1.0000
         0
k =

     []
```

## 5. Tranformada de Laplace en MatLab 
Transforme al dominio s: 8sen(4t)-5cos(4t)

-Codigo 
```
syms ts
y=8*sin(4*t)-5*cos(4*t);
Y= laplace(y)
Y =
32/(s^2 + 16) - (5*s)/(s^2 + 16)

```
Entonces:

$L\left[8sen(4t)-5cos(4t)\right]=\frac{32}{s^2+16}-\frac{5s}{s^2+16}$

### 5.1. Transformada inversa de LaPlace
Obtener la transformada inversa de:
$Y(s)=\frac{6s-4}{s^2+4s+20}$

-Codigo 
```
syms ts
Y=(6*s-4)/(s^2+4*s+20);
y=ilaplace(Y)
y=
6*exp(-2*t)*(cos(4*t) - (2*sin(4*t))/3)

```
Entonces:

$L\left[\frac{6s-4}{s^2+4s+20}\right]=6e^{-2t}cos(4t)-4e^{-2t}sen(4t)$

## 6. Solución de ecuaiones diferenciales 

### 6.1. Metodología de Solución 

-Aplicar transforma de LaPlace a toda la ecuación, para obtener toda la ecuación de en el dominio de s. 

-Despejar la variable que representa la salida de la ecuación.

-Aplicar la inversa de LaPlace a la expresión obtenida para volver al dominio del tiempo.

💡 Ejermplo 4.

$$\ddot{x}+3\dot{x}+2x=0$$.

$x(0)=a, \dot{x}=b$

-Aplicando transformada de LaPlace 
$\left[s^2X(s)-sx(0)-\dot{x}(0)\right]+3\left[sX(s)-x(0)\right]+2X(s)=0$

-Reemplazando condiciones iniciales

$\left[s^2X(s)-as-b\right]+3\left[sX(s)-a\right]+2X(s)=0$

-Despejando X

$\left(s^2+3s+2\right)X(s)=as+b+3a$

-Solución en dominio s

$X(s)=\frac{as+b+3a}{\left(s^2+3s+2\right)}=\frac{2a+b}{s+1}-\frac{a+b}{s+2}$

-Solución en dominio t

$\left(2a+b\right)e^{-t}-\left(a+b\right)e^{-2t}$

## 6.2. Solucion usando MatLab 

```
syms y(t)
eqn = diff(y, t) + 2*y ==5;
condl = y(0) == 2;
sol = dsolve(eqn, condl);
disp(sol);
5/2 - exp(-2*t)/2
```
-Solución

$$y\left(t\right)=\frac{5}{2}-\frac{1}{2}e^{-2t}$$

## 7. Ejercicios 
📚Ejercico 1.
Usando Matlab determinar la solución de la siguiente ecuación diferencial:

$x(t)=8\ddot{x}+4x=8$

$x(0)=5, \dot{x}=1$

```
syms x(t)
 eqn=8*diff(x,t,2)+4*x==8;
dx=diff(x,t);
 ic=[dx(0);x(0)]==[1;5];
 sol=dsolve(eqn,ic);
 disp(sol);
3*cos((2^(1/2)*t)/2) + 2^(1/2)*sin((2^(1/2)*t)/2) + 2
```

📚Ejercico 2.
Usando Matlab determinar la transformada inversa de:

$$Y(s)=\frac{4*s+8}{3s^2+2s+5}$$

```
syms t s
Y=(4*s+8)/(3*s^2+2*s+5);
y=ilaplace(Y);
y =
 
(4*exp(-t/3)*(cos((14^(1/2)*t)/3) + (5*14^(1/2)*sin((14^(1/2)*t)/3))/14))/3
```

Entonces:

$$L^{-1}\left[\frac{4s+8}{3s^2+2s+5}\right]=\frac{4 \cdot e^{-\frac{t}{3}} \left( \cos\left(\frac{\sqrt{14} \cdot t}{3} \right) + \frac{5 \cdot \sqrt{14} \cdot \sin\left(\frac{\sqrt{14} \cdot t}{3} \right)}{14} \right)}{3}$$

## 8. conclusiones 
- MATLAB es una herramienta eficiente para automatizar la solución de ecuaciones diferenciales y fracciones parciales
  
- La transformada de Laplace y su inversa simplifican la resolución de ecuaciones diferenciales, permitiendo transformar el problema del dominio del tiempo al dominio de s, donde las ecuaciones son más fáciles de manejar algebraicamente, y luego revertir el proceso para obtener la solución en el tiempo







