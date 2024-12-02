# Modelamiento de sistemas dinámicos con diagramas de bloques.(Diego Avila, Santigo Garcia)

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






















