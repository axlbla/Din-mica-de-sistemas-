# Trabajo, Energía y Potencia 
En esta clase nos dieron una breve introducción a los movimientos rotacionales y lineales. Aunque no vimos muchos ejemplos ni un análisis muy profundo, tenían un gran parecido con los sistemas mecánicos y se basaban en la física mecánica, solo que en esta ocasión se agregaron las características dinámicas.

## 1.Sistemas Rotacionales 

El análisis es muy parecido al de un sistema mecánico, pero ahora, en lugar de un movimiento lineal, se trata de un movimiento rotacional.

### 1.1.Adaptación de bases matemáticas

 $$F_{R}= K_{2} * y(t)$$ --> $$F_{R}= K_{2} * \phi$$ --> $$\phi$$ es el angulo de torsion
 
 $$F_{F}= K_{1} * y^{'}(t)$$ --> $$F_{F}=b * \phi^{'}$$ --> $$\phi^{'}$$ es la velocidad angular

 $$F= m*a$$ --> $$T= J * \phi^{''}$$ --> J es el momento de inercia 

 ### 1.2.Análisis de sistemas

Muy parecido a los otros sistemas, primero se realiza un diagrama de cuerpo libre y se genera la ecuación representativa, teniendo en cuenta que $$T(t)$$ es la entrada del sistema, y que $$F_{R}$$ y $$F_{F}$$  se oponen a dicha entrada.

  💡**Ejemplo 2:**

  ![image](https://github.com/user-attachments/assets/05f424cb-f9c4-49af-b40f-fd95a6915128)

  **Diagrama de cuerpo libre:**

  ![image](https://github.com/user-attachments/assets/b5ed2526-764c-4e1c-9da1-f4181296cde7)

**Análisis de sistema**

$$T _{t} -F _{F}-F _{R}=j *a$$ --> Aceleración angular

$$T {(t)} -k * \theta(t) -b *\frac{d\theta (t)}{dt}=J *\frac{d^{2}\theta(t) }{dt^{2}}$$

## 2.Definiciones 

>🔑*Trabajo:* Es una medida de la relación del esfuerzo.
>
>$$W=fx  N-m$$
>$$W=\frac{1}{2}kx^{2}$$
>
>🔑*Energía:*Capacidad para realizar el trabajo. Existen dos tipos de energías.
>
>*Energía potencial
>
>*Energía Cinetica
>
>>🔑*Energía Potencial:* La energía potencial varía según la posición respecto a una referencia. Los elementos que almacenan este tipo de energía son los resortes y las masas.
>>
>>$$U=mgh$$
>>
>>La energía potencial en un resorte con características dinámicas es:
>>
>>$$P=kxx^{'}=U^{'}$$
>>
>>🔑*Energía Cinetical:*La energía cinética se da por la velocidad. Solo los cambios de inercia producen esta energía, como lo pueden ser fuerzas de aceleración o desaceleración.
>>
>>$$T=\frac{1}{2}mv^{2}=\frac{1}{2}J\theta ^{2}$$
>>
>🔑*Potencia:*La realización del trabajo que varía con respecto al tiempo.
>
>>La potencia en una masa es:
>>
>>$$P=mx^{''}x^{'}=T^{'}=m *a *v$$
>🔑*Energía disipada:*Los amortiguadores disipan energía y potencia. Sus representaciones matemáticas son:
>>
>> $$P=bx^{'2}$$

## 3.Análisis algebraico para obtener las ecuaciones de energía.

Para estos análisis se supone que el sistema conserva la energía. La fricción se disipa en forma de calor. Los sistemas que no tienen fricción son sistemas conservativos.

### 3.1.Sistemas conservativos 

>🔑*sistemas conservativos:*Todas las clases de energía existentes en el sistema se manifiestan como movimientos o trabajo mecánico.
>
>$$\bigtriangleup(T+U)=\bigtriangleup\omega=0$$
>
Para realizar el análisis, es muy parecido al sistema mecánico. Se formulan unas ecuaciones por medio de un análisis de diagrama de cuerpo libre. Después de formular las ecuaciones, se aplican las características dinámicas y se obtiene la(s) ecuación(es) para el sistema.

💡**Ejemplo 1:**

![image](https://github.com/user-attachments/assets/79e09adf-6ab4-4da2-93a4-dc303710dbc8)

El análisis nos da la siguiente ecuación, teniendo en cuenta las propiedades de los elementos.

$$T+U=\frac{1}{2}mx^{'2} + \frac{1}{2}k * x^{2}$$

Después se deriva para obtener la energía total del sistema, quedando:

$$\frac{1}{2}mx^{''}+kx=0$$

## 4.Conservación del movimiento translacional-rotacional

En esta parte de la clase se mostró el proceso para formular ecuaciones para sistemas que tengan movimientos rotacionales y los transformen en movimientos translacionales, como lo puede ser un motor moviendo cargas por medio de una cremallera o bandas.

También se enseñaron los casos más frecuentes y las representaciones dinámicas de los elementos de estos sistemas, como lo son la tensión, el torque y la distancia angular:

### 4.1.Tensión

$$T=mr^{2} \ frac{d^{ \theta '2}}{dt^{2}}$$

### 4.2.Torque 

$$T=J \frac{d^{2}{ \theta } }{dt^{2}}$$

### 4.2.Distancia Angular

$$\theta=\frac{{y} }{r}$$

### 4.3.Análisis de sistema

Muy parecido a los otros sistemas, se hace un diagrama de cuerpo libre y se comienzan a generar las ecuaciones de modelación algebraica según las propiedades y normas dadas por los elementos. Después, se agregan las características dinámicas.

💡**Ejemplo 1:**

![image](https://github.com/user-attachments/assets/f1c6e48f-b918-450f-b922-d2717ff49cfd)

#### 4.3.1.Análisis de cuerpo libre

![image](https://github.com/user-attachments/assets/5342f65f-7d3a-44f0-b3cf-b75b68f87669)

#### 4.3.2.Análisis y generación de ecuaciones"

$$T_{m}- T _{1} - B _{m}\frac{d\theta }{dt} = J _{m}\frac{d^{2}\theta }{dt^{2}}$$

Después de introducir las características dinámicas en el sistema, tenemos:

$$T_{m}- Mr\frac{d^{2}y}{dt^{2}} - \frac{B _{m}}{r}\frac{dy }{dt} = \frac{J _{m}}{r}\frac{d^{2}y }{dt^{2}}$$

## 5.Sistemas Electricos 

Para el análisis de estos tipos de circuitos, nos apoyamos en las leyes de Kirchhoff junto con las características dinámicas de cada uno de sus componentes, como lo son condensadores, bobinas o resistencias.

### 5.1.Redes RLC

Circuitos pasivos compuestos por condensadores, resistencias y bobinas. 

#### 5.1.1.Resistencias 

$$R=\frac{v _{t}}{i _{t}}$$--> Ley de ohm

#### 5.1.2.Bobinas 

$$v _{t}=L\frac{di _{t}}{dt}$$--> Carga de inductor 

#### 5.1.3.Condensadores

$$i _{t}=C\frac{dv _{t}}{dt}$$

### 5.2.Análisis de circuitos 

Para realizar el análisis, primero se debe escoger uno de los dos métodos para aplicar las leyes de Kirchhoff, ya sea mallas o nodos. Después, se generan la(s) ecuación(es) correspondiente(s) del circuito RLC. Al terminar de generar las ecuaciones, se cambian las variables estáticas por las dinámicas y se realizan los respectivos análisis para que la(s) ecuación(es) quede(n) en términos de tensión o corriente, y también para que quede en términos de la entrada y la salida (normalmente es una tensión o una corriente del circuito).

💡**Ejemplo 1:**

![image](https://github.com/user-attachments/assets/19fa1177-829d-4a97-867f-cfd830db222a)

En este caso, vamos a aplicar el método de mallas para el análisis del circuito, dándonos la siguiente ecuación:

$$-u _{t}+ v _{R} +v _{L} +v _{C}=0 $$

Después de obtener la ecuación, reemplazamos por las características dinámicas de los componentes:

$$-u _{t}+ i _{t}* R +L \frac{di _{t}}{dt} +y _{t}=0$$

Se deja en términos de la variable $$y _{t}$$ por medio de un análisis del sistema, quedando:

$$i _{t}=C \frac{dy _{t}}{dt}$$

$$-u _{t}+RC \frac{dy _{t}}{dt} +LC\frac{d(\frac{C \frac{dy _{t}}{dt}}{dt})}{dt}+y _{t}=0$$

Haciendo álgebra para simplificar la ecuación, queda:

$$-u _{t}+RC \frac{dy _{t}}{dt} +LC\frac{d^{2}y _{t}}{dt^{2}}+y _{t}=0$$


💡**Ejemplo 2:**

![image](https://github.com/user-attachments/assets/61f68b45-6a49-40d4-b8c2-fb945c5931ea)

En este caso, aplicaremos la ley de Kirchhoff de nodos, dándonos la ecuación de la siguiente manera:

$$i _{u}-i _{1}-i _{c} = 0$$

Se llevan todas las corrientes en términos de voltajes.

$$i _{u}-\frac{V _{AB}}{0.5}-2 \frac{dy _{t}}{dt} = 0$$

Se hace un análisis conn $$V _{AB}$$ para dejarlo todo en términos de la salida y la entrada, quedando:

$$V _{AB}=i _{c} * 1+ y _{t}$$

$$V _{AB}=2 \frac{dy _{t}}{dt}*1 +y _{t}$$

$$i _{u}-\frac{2 \frac{dy _{t}}{dt}*1 +y _{t}}{0.5}-2 \frac{dy _{t}}{dt} = 0$$

Haciendo álgebra para simplificar la ecuación, tenemos:

$$U _{t}-6\frac{dy _{t}}{dt}-2 y _{t} = 0$$

## 5.Conclusión

En esta clase se aprendió a modelar los sistemas rotacionales y translacionales. También vimos circuitos eléctricos RLC, aplicando leyes vistas en otras materias para así generar ecuaciones que representen los sistemas con sus características dinámicas, aprendiendo el análisis básico de elementos presentes tanto eléctrica como mecánicamente.
