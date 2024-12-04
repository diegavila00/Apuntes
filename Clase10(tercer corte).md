# Modelamiento de sistemas dinámicos con diagramas de bloques.(Diego Avila, Santigo Garcia)
En esta clase vimos cómo funcionan y como se modelan algunos sistemas electromecánicos, como solenoides, motores de corriente continua y engranajes. Vimos como se hace paso a paso y cómo se relacionan las partes eléctricas, mecánicas y electromagnéticas de estos sistemas, y cómo representarlas con diagramas de bloques para entender mejor su comportamiento. Todo esto se hace utilizando ecuaciones matemáticas y transformadas de Laplace, herramientas clave para analizar y diseñar dispositivos que vemos en la industria y la tecnología actual.
## 1.Solenoide
Formado por un circuito electrico, acoplamiento electromecanico y un sisetma mecanico de trasnlación.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/s1.png)

- Modelamiento Electrico

![](https://github.com/diegavila00/Apuntes/blob/main/TP/eeee.png)

$L\left(\frac{di}{dt}\right)+R_i=V(t) \rightarrow L_sI(s)+RI(s)=V(s)$

$I(s)=V(s)\left(\frac{1}{L_s+R}\right) \rightarrow \frac{I(s)}{V(s)}=\frac{1}{L_s+R}$

>🔑 El electroimán produce una fuerza mecanica proporcional a la corriente.
>$(K_s)$

- Acolple entre la parte electromecánica y la parte mecánica.

El electroimán trae una masa acoplada por medio de un resorte y se concidera el amortiguamiento dado por la envolvente de la bobina.

$m\left(\frac{d^2x}{dt^2}\right)+b\left(\frac{dx}{dt}\right)+kx=f(t)$

$mS^2X(s)+bSX(s)+kX(s)=F(s)$

$X(s)[mS^2+bS+k]=F(s)$

$X(s)=\frac{F(s)}{mS^2+bS+k}$

$\frac{X(s)}{F(s)}=\frac{1}{mS^2+bS+k}$

- Representación en diagrama de bloques.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/dg.png)

- Multiplicación

![](https://github.com/diegavila00/Apuntes/blob/main/TP/dg2.png)

## 2. Motor DC

![](https://github.com/diegavila00/Apuntes/blob/main/TP/motor.png)

## 2.1 Corriente de campo 

- Circuito Electromagnético

$L_c\frac{di_c}{dt}+R_c(i_c)=V_c(t)$

$I_c(s)=V_c(s)\frac{1}{(sL_c+R_c)}$

- El flujo ($\Phi$) en el entre hierro es proporcional a la corriente de campo
  
$\phi=K_c(i_c)$

- El torque desarrollado es proporcional al $\Phi$ y a la corriente de armadura

$T_m=K_a i_a(t) K_c i_c(t)$

$T_m(s)=(K_a K_c i_a)i_c(s)=K_m i_c(s)$

- El torque aplicado a la carga es el desarrollado por el motor menos la inercia de la carga

$T_c(s)=T_m(s)-T_p(s)$

- Parte mecanica

$J\left(\frac{d^2\theta}{dt^2}\right)+b\left(\frac{d\theta}{dt}\right)+K\theta=\tau(t)$

$\Theta(s)=T_c(s)\left(\frac{1}{(s^2 J+bs)}\right)$

$\Theta(s)=V_c(s)\frac{K_m}{(sL_c+R_c)(Js^2+bs)}-T_p(s)\frac{1}{(J^2+bs)}$

$\frac{\Theta(s)}{V_c(s)}=\frac{K_m}{(sL_c+R_c)(Js^2+bs)}$

- Diagrama de bloques

![](https://github.com/diegavila00/Apuntes/blob/main/TP/dm.png)

## 3. Engranajes 

![](https://github.com/diegavila00/Apuntes/blob/main/TP/engranajes.png)

$\frac{\tau_2}{\tau_1}=\frac{N_2}{N_1}$

$\frac{N_2}{N_1}=-\frac{\theta_1}{\theta_2}$

- J y $K_m$ cambian si se tiene en cuenta el efecto de los engranajes o poleas

$\frac{\Theta(s)}{Vc(s)}=\frac{K_m}{(sL_c+R_c)(Js^2+bs)}$

$\beta_{equiv}=\left(\frac{N_1}{N_2}\right)^2\beta$

$J_{equiv}=\left[JN_1+\left(\frac{N_1}{N_2}\right)^2(J+JN_2)\right]$

- Diagrams de bloques

![](https://github.com/diegavila00/Apuntes/blob/main/TP/engranajes%201.0.png)

💡Ejemplo 1.

- Modelar el sistema usando diagramas de bloques

![](https://github.com/diegavila00/Apuntes/blob/main/TP/amplificador.png)

- Solución

![](https://github.com/diegavila00/Apuntes/blob/main/TP/me.png)

## 4. Ejercicios

📚 Ejercico 1. 

- Realizar el modelamiento del siguiente circuito usando diagramas de bloques.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/circuito2.png)

- Diagrama de bloques

![](https://github.com/diegavila00/Apuntes/blob/main/TP/mc.png)

![](https://github.com/diegavila00/Apuntes/blob/main/TP/mc2.png)

## 5. Conclusiones 

- Los diagramas de bloques son herramientas muy útiles para simplificar sistemas complejos como motores, solenoides o engranajes. Nos permiten visualizar claramente cómo se conectan las partes eléctricas, mecánicas y electromagnéticas, haciendo más fácil entender su funcionamiento y comportamiento.

- En los sistemas dinámicos, cada componente influye en el otro. Por ejemplo, en un solenoide, la corriente genera una fuerza, que a su vez mueve una masa. Es como un efecto dominó, y las ecuaciones matemáticas nos ayudan a describir esas relaciones paso a paso.

- Aunque a veces parezcan complicadas, las ecuaciones y las transformadas de Laplace son fundamentales para modelar estos sistemas. Nos ayudan a predecir cómo van a funcionar en diferentes situaciones, lo que es clave para diseñar dispositivos tecnológicos eficientes y fiables. 


## 6. Referencias 

- Rebollo, S. E. [@ser7620]. (s/f). Función de transferencia a partir de diagramas de bloques circuito RLC. Youtube. Recuperado el 4 de diciembre de 2024, de https://www.youtube.com/watch?v=6ADkXXKGSqA

- Ogata, K. (2003). Ingeniería de control moderna. Pearson educación.




















