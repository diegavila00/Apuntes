# Modelamiento de sistemas dinámicos con diagramas de bloques.(Diego Avila, Santigo Garcia)

## Solenoide
Formado por un circuito electrico, acoplamiento electromecanico y un sisetma mecanico de trasnlación.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/s1.png)

- Modelamiento Mecanico

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































