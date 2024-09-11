# Ecuaciones Diferenciales y metodo resumido de tranformda de Laplace 
Antes de empezar con la solucion de ecuaciones diferenciales y el metodo resumido para la solución de tranformada de Laplace, terminados de repasar los dos casos de descomposición en fracciones parciales que faltaron de la clase anterior los cuales son cuando el Tiene raices reales reptidas y cuando las raices son complejas, tambien aprendimos como solucionar fraciones parciales, la transformada y la transformada inversa de Lplace, ecuaciones diferenciales usando matlab.

## 1. Caso 2 fraciones parciales(n raices reales repetidas)
$G(s)=\frac{P(s)}{Q(s)}=\frac{P(s)}{(s+p)^n}$
- 
-Descomposición

$G(s)=\frac{A}{(s+p)}+\frac{B}{(s+p)}+......+\frac{N}{(s+p)^n}$

💡Ejemplo 1. 

$G(s)=\frac{2s^2+6s+5}{(s+2)(s+1)}=\frac{A}{S+2}+\frac{B}{s+1}+\frac{C}{(s+1)^2}$

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


$\frac{A}{S+2}+\frac{B}{s+1}+\frac{C}{(s+1)^2}=\frac{1}{S+2}+\frac{1}{s+1}+\frac{1}{(s+1)^2}$

-Solución aplicando transformada de Laplace 

$L^{-1}=e^{-2t}+e^{-t}+te^{-t}$
-
