# Trabajo energia y potencia
En esta clase vimos cómo funcionan conceptos básicos como el trabajo, la energía y la potencia en los sistemas mecánicos. vimos términos importantes como la energía potencial (la que tiene un objeto por estar en una posición) y la energía cinética (la que tiene por moverse), y cómo estas se aplican a cosas como resortes, masas y amortiguadores. También vimos sobre cómo se conserva la energía en los sistemas y cómo podemos usar ecuaciones matemáticas para describir el movimiento de distintos tipos de sistemas, tanto en línea recta como en rotación.

## 1. Coceptos importantes

- Trabajo: Es una medida de la realización de la fuerza.

$W=FX$

Trabajo total realizado:

$\int_{0}^{x} kx \cdot dx= \frac{1}{2}kx^2$

- Energía: Capacidad para realizar trabajo.
  - Energía potencial.
  - Energia cinética.

- Energía potencial: La energía cinénitca es equivalente al trasbajo realizado por la fuerza externa.
  - En los sistemas mecanicos los resortes y las masas almacenan energia potencial.
  - En los sietmsa mecanicos la energia potencial cambia de acuerdo asu posición.
    
  $U=mgh$

- Energía cinética: Se debe a la velocidad.
  - Solamente los elementos de inercia pueden almacenar energía cinética.
  - Lineal:   

$T=\frac{1}{2}mv^2$               
  
- Rotacional:

$T=\frac{1}{2}j\dot{\theta}^2$

- Cambio de energía cinética lineal:

$\frac{1}{2}mv_{2}^2-\frac{1}{2}mv_{1}^2$

- Cambio de energía cinética rotacional:

$\frac{1}{2}j\dot{\theta}_{2}^2-\frac{1}{2}j\dot{\theta}_1^2$

- Potencia: variación de trabajo con respecto al tiempo.

$P=\frac{dw}{dt}$


## 2. Aplicación en elementos mecanicos.

- Energia potencila en un resorte: Es el tranajo neto hecho sobre el resorte por las fuerzas que actuan en sus extremos.

$U=\int_{0}^{x} kx \cdot dx=\frac{1}{2}kx^2$

>🔑 x= distancia 

- Cambio de energía

$\triangle U=\int_{x_{1}}^{x_{2}} kx\cdot dx =\frac{1}{2}kx_2^2-\frac{1}{2}kx_1^2$


- Potencia en un resorte: Potencia requierida para estirar o contrear un resorte:

$P=\frac{dw}{dt}F=\frac{dx}{dt}=F\dot{x}=Kx\dot{x}$

>🔑 Teniendo en cuenta que:
>$U=\frac{1}{2}mx^2$

$P=kx\dot{x}=\dot{U}$

- Potencia en una masa: La potencia requerida para acelerar una masa en línea recta.
  
$P=m\ddot{x}\dot{x}$

>🔑 Teniendo en cuenta que:
>$T\frac{1}{2}mv2$

$P=\dot{T}$

- Energía dispersada (Sobre elemento con fricción)

$\triangle W=b\int_{b_1}^{b_2}\dot{x}^2 \cdot dt $

- Potencia disipada en amortiguador de cilindro:

$P=b\dot{x}^2$

## 3. Obtención de las ecuaciones de movimieto

- Conservación energía: Es posible obtener el modelo matemático considerando que la energía total de un sistema permanece igual si ninguna energía entra o sale del sistema

Sistemas conservativo (No se dispersa energía)

$\triangle (T+U)=\triangle W \rightarrow$ trabajo neto

si no entra energía externa entonces:

$T+U= constante$

💡Ejemplo 1.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/1.png)

$T=\frac{1}{2}m\dot{x}^2$

$U=\frac{1}{2}kx^2$

$T+U=\frac{1}{2}m\dot{x}^2+\frac{1}{2}kx^2 = constante$

$\frac{d}{dt}(T+U)=m\dot{x}\ddot{x}+kx\dot{x}=(m\ddot{x}+kx)\dot{x}=0$

$m\ddot{x}+k\dot{x}=0$


💡Ejemplo 2. 

![](https://github.com/diegavila00/Apuntes/blob/main/TP/2.png)

$U_0=mgx_0+\frac{1}{2}k\delta^2$

$k\delta= mg \rightarrow$ en equilibrio

>🔑
>$\delta$
> es el cambio de posición debido a la posición inical 

$U=mg(x_0-x)+\frac{1}{2}kx^2$

$T=\frac{1}{2}kx^2$

$\frac{d}{dt}(T+U)=m\dot{x}\ddot{x}+kx\dot{x}=0$

$m\ddot{x}+kx=0$
-

📚 Ejercico 1. 

![](https://github.com/diegavila00/Apuntes/blob/main/TP/3.png)

- Desarrollo

$J\ddot{\theta}=(T_1-T_2)R$

$m\ddot{x}=-T_1$

$M\ddot{y}=-ky+T_1+T_2$

>🔑
>$x=2y$,
>$R\theta=x-y=y$,
>$J=\frac{1}{2}MR^2$

$\frac{1}{2}MR^2\ddot{\theta}=\frac{1}{2}MR\ddot{y}=(T_1-T_2)R$

$m\ddot{x}=-T_1$

$M\ddot{y}+ky=T_1+T_2$

$\frac{1}{2}M\ddot{y}+M\ddot{y}+ky=2T=-2m\ddot{x}$

$\frac{3}{2}M\frac{\ddot{x}}{2}+k\frac{x}{2}=-2m\ddot{x}$

$(m+\frac{3}{8}M)\ddot{x}+\frac{1}{4}kx=0$
-

## 4. Conclusiones 

1. En los sistemas mecánicos conservativos (sin pérdida de energía), la suma de la energía cinética y potencial permanece constante. Esto significa que la energía total no cambia a menos que se introduzcan fuerzas externas o disipación.
2. El trabajo realizado sobre un objeto está directamente relacionado con el cambio en su energía. La energía cinética cambia con la velocidad del objeto, mientras que la energía potencial depende de su posición en un campo de fuerzas, como la gravedad o un resorte.
3. La potencia mide la velocidad a la que se realiza el trabajo o se transfiere la energía en un sistema. Esto es crucial para entender el rendimiento de los sistemas mecánicos, ya que permite calcular cuánta energía se utiliza o disipa en un tiempo determinado, afectando la eficiencia total del sistema.

>🔑 Diego Avila
>y
>Santigo Garcia 

## 5. Referencias 

- Ogata, K., & Sanchez, G. L. P. (1987). Dinámica de sistemas (Vol. 3). Prentice-Hall Hispanoamericana.
- Ogata, K. (2003). Ingeniería de control moderna. Pearson educación. 


