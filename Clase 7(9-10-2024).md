# Sistemas Eléctricos 
En la clase de hoy vimos como se hace el analisis de un circuito RLC. que tiene tres componentes básicos: una resistencia (R), una bobina o inductor (L) y un condensador (C). Estos circuitos se usan mucho para filtrar señales, ajustar frecuencias y en sistemas de radio o telecomunicaciones. El comportamiento de un circuito RLC se explica por las leyes de Kirchhoff, que dicen cómo se relacionan la corriente y el voltaje en el circuito. Según los valores de estos tres elementos, el circuito puede reaccionar de diferentes formas, como más rápido o más lento, dependiendo de la situación.

## 1. Circuto RLC
Las leyes de Kirchhoff se encaragan de modelar el comportamiento de los circuitos, de las cuales para los curcuitos RLC usaremos las siguientes:


- En resistencia(Ley de Ohm)

![](https://github.com/diegavila00/Apuntes/blob/main/TP/R.png)

$V(t)=i(t)R$

- En Condensador(Carga de un condensador)

![](https://github.com/diegavila00/Apuntes/blob/main/TP/C.png)

$i(t)=C\dot{vC}$

$VC=\frac{1}{C}\int iC\cdot dt$

- En un inductor

![](https://github.com/diegavila00/Apuntes/blob/main/TP/L.png)

$V(t)=L\dot{iL}$

💡Ejemplo 1.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/m.png)

$-U+iR+L\dot{iL}+y=0$

$-U+RC\dot{vC}+\frac{Ld}{dt}\left(\frac{Cdy}{dt}\right)+y=0$

$-U+RC\dot{vC}+LC\left(\frac{dy^2}{dt^2}\right)+y=0$

💡Ejemplo 2.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/D.png)

$V=VR_1+VR_2++VC$

$V=CR_1\frac{dVc}{dt}+CR_2\frac{dVc}{dt}+VC$

$V=(R_1+R_2)C\frac{dVc}{dt}+VC$

$$IR_1+IR_2 $$

$$ \frac{V-y}{R_1}=\frac{y-VC}{R_2}$$

$$\left(\frac{V-y}{R_1}\right)R_2=y-VC $$

$$ VC= y-\left(\frac{V-y}{R_1}\right)R_2$$

$$ \frac{dVc}{dt}=\dot{y}-\left(\frac{\dot{V}-\dot{y}}{R_1}\right)R_2$$

$V=(R_1+R_2)\left(\dot{y}-\left(\frac{\dot{V}-\dot{y}}{R_1}\right)R_2\right)+y-\left(\frac{V-y}{R_1}\right)$
-

💡Ejemplo 3.


![](https://github.com/diegavila00/Apuntes/blob/main/TP/EEE.png)

$I_{ei}-I_2-I_1=0$

$\frac{e_i-VT}{R_1}-C_1-\dot{VT}-C_2\dot{e_o}$

$$VT=I_1*R_2+e_o $$

$$VT=R_2C_2\dot{e_o}+e_o$$

$$\dot{VT}=R_2C_2\ddot{e_o}+\dot{e_o}$$

$\frac{e_i-R_2C_2\dot{e_o}+e_o}{R_1}+C_1R_2C_2\ddot{e_o}+e_{e_o}-C_2\dot{e_o}$
-

## 2. Ejercicios 

📚 Ejercico 1.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/FFFFF.png)

$i(t)=i_{L(t)}+i_{R(t)}+i_{C(t)}$

$i_{L(t)}+\frac{V(t)}{R}+C\dot{V}_{(t)}$

$V(t)=V_{L(t)}=L\dot{i}_{L(t)}$

$\ddot{i_{L(t)}}+\frac{L}{R}\dot{i_L(t)}+i_{L(t)}=i_{(t)}$


## 3. Conclusiones 

- La resistencia (R) controla la rapidez con que el sistema alcanza el equilibrio, influyendo en si el circuito oscila más o menos antes de estabilizarse.

- En un circuito RLC, la energía se intercambia entre el condensador y el inductor, mientras que la resistencia disipa parte de esa energía en forma de calor.

>🔑 Diego Avila
>y
>Santigo Garcia


## 4. Referencias 
- Ogata, K. (2003). Ingeniería de control moderna. Pearson educación.
- Chen, C. T. (1995). Analog and digital control system design: transfer-function, state-space, and algebraic methods. Oxford University Press, Inc..
- Bibliografía
Circuito eléctrico de segundo grado – Circuito RLC. (2022, enero 21). dademuchconnection. https://dademuchconnection.wordpress.com/2022/01/21/circuito-electrico-de-segundo-grado-circuito-rlc/












