# Amplificadores operacionales y sistemas hidráulicos y sistemas térmicos 
En esta clase terminamos de ver modelamiento de sistemas electricos analizando el amplificadorn operacional y algunas de sus configuraciones, tambien vimos como se debe hacer el analisisi para los sietmas hidráulicos y termicos, entiendo cuales son las ecuaciones que se utilizan para el modelamiento de estos.

## 1. Amplificador no inversor 


![](https://github.com/diegavila00/Apuntes/blob/main/TP/am.png)

- La tension en la entrada inversora(V-) y la entrada no inversora(V+) es igual.
- la corriente en las dos entradas es 0.
- La impedancia de entrada tiende a infinito.
- la impedancia de salida tiende a 0.

💡Ejemplo 1.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/ammm2.png)

$i_1-i_2=0$

$\frac{e_o-e_i}{R_2}-\frac{e_i}{R_1}=0 $

$\frac{e_o}{R_2}=e_i\left(\frac{1}{R_2}+\frac{1}{R_1}\right)$

$e_o=e_i\left(1+\frac{R_2}{R_1}\right)$

>🔑 De esta manera se puede dterminar la ganancia del amplificador no inversor

## 2. Amplificadores con elementos almacenadores de energia

💡Ejemplo 2.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/ammmm3.png)

$i_1-i_2-i_3=0$

$\frac{e_i-e'}{R_1}-\frac{e'-e_o}{R_2}-C\frac{d(e'-e_o)}{dt}=0$

$$e'=0$$

>🔑La tension en el punto e' es 0 debido que la entrada no inversora(V+)esta conecatda a 0 voltios, recordemos que la tension en las dos entradas del amplificador simepre va a ser la misma 


$\frac{e_i}{R_1}-\frac{-e_o}{R_2}-C\frac{d(-e_o)}{dt}=0$

$\frac{e_i}{R_1}=-\frac{e_o}{R_2}-C\frac{d(e_o)}{dt}$


## 3. Sistemas hidráulicos 
### 3.1 Sistemas de tanques 
En sistemas industriales de tanques el objetivo es mantener un flujo constante 

![](https://github.com/diegavila00/Apuntes/blob/main/TP/h.png)

- qi: Flujos de entrada y salida de líquido
- R1: Resistencia al flujo
- A1: Área transversal del tanque
- h1: Nvel de liquido en el tanque

Ecuaciones 
-

- Flujo de salida del tanque 

$q_i=\frac{h_1}{R_1}$

- Intercambio de energia

$A_1\dot{h}_1=q_i-q_1$

Modelo qi como entrada y q1 como salida 
-

$$ q_1=\frac{h_1}{R_1}$$

$$ A1\dot{h}_1=q_i-q_1$$

$$ h_1=q_1*R_1$$

$$R_1* A_1*\dot{q}1=q_i-q_1$$

💡Ejemplo 3.

![](https://github.com/diegavila00/Apuntes/blob/main/TP/T.png)

- Tanque 1

$R_1A_1\dot{q}_1=q_i-q_1$

- Tanque 2

$R_2A_2\dot{q}_2=q_1-q_2$

$q_1=q_2+R_2A_2\dot{q}_2$

$\dot{q}_1=dot{q}_2+R_2A_2\ddot{q}_2$

$R_1A_1(\dot{q}_2R_2A_2\ddot{q}_2)=q_i-(q_2+R_2A_2\dot{q}_2)$
-

## 4. Sistemas térmicos  

![](https://github.com/diegavila00/Apuntes/blob/main/TP/s.png)

- Ecuaciónes

$R=\frac{\theta}{h}_o$

$Cd\theta=(h_i-h_o)dt$

- Modelamiento

$Cd\theta=h_i-h_o$

$RC\frac{d\theta}{dt}+\theta=Rh_i$

## 5. Ejercicios 

📚 Ejercico 1. 

![](https://github.com/diegavila00/Apuntes/blob/main/TP/zzzzzzz.png)

$pq_1(t)=p\left(\frac{dV_1}{dt}\right)=pA_1\left(\frac{dh_1}{dt}\right)$

$pq(t)-pq_1(t)-pq_2(t)=p\left(\frac{dV_2}{dt}\right)=pA_2\left(\frac{dh_2}{dt}\right)$

$$q_1(t)=\frac{h_2(t)-h_1(t)}{r_1}$$

$$q_2(t)=\frac{h_2(t)-0}{R_2}$$

$R_1A_1\frac{dh_1}{dt}+h_1=h_2$

$R_1R_2A_1\frac{dh_2}{dt}+h_2(R_1+R_2)=R_2h_1+qR_2R_1$

## 6. Conclusiones 
- El amplificador no inversor permite amplificar la señal de entrada con una ganancia controlada por 1+R2/R1, facilitando el análisis del comportamiento de los circuitos y el diseño de sistemas de mayor precisión.
- anto en sistemas hidráulicos como térmicos, el modelamiento se basa en el equilibrio de flujos o transferencia de energía, lo cual permite analizar y controlar la dinámica de estos sistemas industriales mediante ecuaciones diferenciales.


>🔑 Diego Avila
>y
>Santigo Garcia


## 7. Referencias 
- Ogata, K. (2003). Ingeniería de control moderna. Pearson educación.
- Chen, C. T. (1995). Analog and digital control system design: transfer-function, state-space, and algebraic methods. Oxford University Press, Inc..
- de Una Tubería Corta, E. 1-T. D. E. A. C. D. A. T. (s/f). MODELAJE DE SISTEMAS HIDRAULICOS. Wordpress.com. Recuperado el 26 de octubre de 2024, de https://guiasusb.wordpress.com/wp-content/uploads/2013/09/ps1316-tema-2-1-sistemas-hidrc3a1ulicos.pdf


















