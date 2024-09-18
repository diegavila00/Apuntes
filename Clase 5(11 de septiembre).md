# Sistemas mecanicos mas complejos 
En esta clase seguimos trabajando con sistemas mecanicos, pero trabajamos con algunos sitemas mecanicos mas complejos y una pequeña introduccion a los sistemas rotacionales.


## 1. Sistemas acoplados 

![](https://github.com/diegavila00/Apuntes/blob/main/TP/acoplados.png)

- Diagrama de cuerpo libre m1 y m2
![](https://github.com/diegavila00/Apuntes/blob/main/TP/m1%20y%20m2.png)

- Desarrollo matematico

- **Para m1**

$\sum f = m*a$

$u-FR_{1}-FR_{2}-FF=m_{1}*a_{m_{1}}$

$u(t)-k_{1}x_{1}(t)-k_{2}[x_{1}(t)-x_{2}(t)]-b\frac{dx_{1}(t)-x_{2}(t)}{dt}=m_{1}\ddot{x_{1}}$

- **Para m2**

$\sum f = m*a$

$FR_{2}+FF-FR_{3}=m_{2}*a_{m_{2}}$

$k_{2}[x_{1}(t)-x_{2}(t)]+b\frac{dx_{1}(t)-x_{2}(t)}{dt}-k_{3}x_{2}=m_{2}\ddot{x_{2}}$

💡Ejemplo 1.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/cuerpo%20libre%20ejercicio%202.1.png)

- Diagrama de cuerpo libre para m1 y m2

![](https://github.com/diegavila00/Apuntes/blob/main/TP/ejemplo.png)

- Desarrollo matematico 

- **Para m1**

$\sum f = m*a$

$FR_{2}-FR_{1}-FF=m_{1}*a_{m_{1}}$

$k_{2}(x_{1}-x_{2})-kx_{1}-k\dot{x}=m_{1}\ddot{x_{1}}$

- **Para m2**

$\sum f = m*a$

$FR_{2}=m_{2}*a_{m_{2}}$
$-k_{2}(x_{1}-x_{2}=m\ddot{x_{2}})$


## 2. Tipos de sistemas 

- SISO (single input - single output)
- MISO (multiple input - single output)
- SIMO (single input - multiple output)
- MIMO (multiple input - multiple output)

## 3. Ejercicos 

📚 Ejercico 1. 

![](https://github.com/diegavila00/Apuntes/blob/main/TP/f.png)

- Diagrama de cuerpo libre m1 y m2

![](https://github.com/diegavila00/Apuntes/blob/main/TP/a.png)

- Desarrollo matematico 

- **Para m1**

$\sum f_{1} = m*a$

$-FK_{1}-FB_{1}+FK_{2}+FB_{2}+F_{1}=m_{1}\ddot{x_{1}}$

$-K_{1}-B_{1}\dot{x_{1}}+k_{2}(x_{2}-x_{1})+B_{2})(\dot{x_{2}}-\dot{x_{1}})+F_{1}=m_{1}\ddot{x_{1}}$

$m_{1}\ddot{x_{1}}+(B_{1}+B_{2})\dot{x_{1}}-B_{2}\dot{x_{2}}+(k_{1}+k_{2})x_{1}-k_{2}x_{2}=F_{1}$


- **Para m2**

$\sum f_{2} = m*a$

$-FK_{2}-FB_{2}-FK_{3}-FB_{3}+F_{2}=m_{2}\ddot{x_{2}}$

$-K_{2}x_{2}+K_{2}x_{1}-B_{2}\dot{x_{2}}+B_{2}\dot{x_{1}}-K_{3}x_{2}-B_{3}\dot{x_{2}}+F_{2}=m_{2}\ddot{x_{2}}$

$m_{2}\ddot{x_{2}}-B_{2}\dot{x_{1}}+(B_{2}+B_{3})\dot{x_{2}}-K_{2}x_{1}+(K_{2}+k_{3})x_{2}=F_{2}$
$

## 4. Conclusiones 
-  Los sistemas mecánicos acoplados muestran cómo las fuerzas y desplazamientos en un cuerpo afectan directamente a otro a través de elementos como resortes y amortiguadores. Las ecuaciones para cada masa demuestran que la dinámica de una depende de la posición y velocidad de la otra, lo que genera una compleja interrelación entre ellas.

- El análisis de estos sistemas requiere el uso de ecuaciones diferenciales que describen el comportamiento de las fuerzas y aceleraciones. A través de estas ecuaciones, es posible predecir el movimiento y las respuestas de los sistemas mecánicos bajo diversas condiciones, lo que es esencial para el diseño y control de estos sistemas.

## 5. Referencias 
- Rebollo, S. E. [@ser7620]. (s/f). Modelado de un sistema masa, resorte, amortiguador de 2 grados de libertad. Youtube. Recuperado el 18 de septiembre de 2024, de https://www.youtube.com/watch?v=_EbaOBDxk1Y

- Ogata, K., & Sanchez, G. L. P. (1987). Dinámica de sistemas (Vol. 3). Prentice-Hall Hispanoamericana.
- Ogata, K. (2003). Ingeniería de control moderna. Pearson educación.














