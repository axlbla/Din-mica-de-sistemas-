# Trabajo, Energia y Potencia 
En esta clase nos dieron una breve introduccion a movimientos rotacionales y movimientos lineales , aunque no vimos muchos ejemplos y tampoco un analisis muy profundo, ya que tenia un gran parecido a los sistemas mecanicos y se basaban en la fisica mecanica , solo que en esta ocacion se agregaron las caracteristicas 
dinamicas.
## 1.Sistemas Rotacionales 

El análisis es muy parecido al del sistema mecánico, pero ahora, en lugar de un movimiento lineal, se trata de un movimiento rotacional.

### 1.1Adaptacion de bases matematicas 

 $$F_{R}= K_{2} * y(t)$$ --> $$F_{R}= K_{2} * \phi$$ --> $$\phi$$ es el angulo de torsion
 
 $$F_{F}= K_{1} * y^{'}(t)$$ --> $$F_{F}=b * \phi^{'}$$ --> $$\phi^{'}$$ es la velocidad angular

 $$F= m*a$$ --> $$T= J * \phi^{''}$$ --> J es el momento de inercia 

 ### 1.2Analisis de sitemas 

Muy parecido a los otros sistemas, primero se realiza un diagrama de cuerpo libre y se genera la ecuación representativa, teniendo en cuenta que $$T(t)$$ es la entrada del sistema, y que $$F_{R}$$ y $$F_{F}$$  se opone a la 
 entrada.

  💡**Ejemplo 2:**

  ![image](https://github.com/user-attachments/assets/05f424cb-f9c4-49af-b40f-fd95a6915128)

  **Diagrama de cuerpo libre:**

  ![image](https://github.com/user-attachments/assets/b5ed2526-764c-4e1c-9da1-f4181296cde7)

**Analisis de sistema:**

$$T _{t} -F _{F}-F _{R}=j *a$$ --> aceleracion angular

$$T {(t)} -k * \theta(t) -b *\frac{d\theta (t)}{dt}=J *\frac{d^{2}\theta(t) }{dt^{2}}$$

## 2.Definiciones 

>🔑*Trabajo:* Es una medida de la relacion del esfuerza
>
>$$W=fx  N-m$$
>$$W=\frac{1}{2}kx^{2}$$
>
>🔑*Energia:*Capacidad para realizar el trabajo,existen dos tipos de energias
>
>*Energia potencial
>
>*Energia Cinetica
>
>>🔑*Energia Potencial:* La energia potencial varia segun la posicion respecto a una referencia,los elementos que almacenan este tipo de enrgia
>>son los resortes y las masas
>>
>>$$U=mgh$$
>>
>>La energia potenical en un resorte con caracteriticas dinamicas es:
>>
>>$$P=kxx^{'}=U^{'}$$
>>
>>🔑*Energia Cinetical:* la energia cinetica se da por la velocidad, solo los cambios de incercia producen esta energia, como lo pueden ser fuerzas de aceleracion o desaceleracion
>>
>>$$T=\frac{1}{2}mv^{2}=\frac{1}{2}J\theta ^{2}$$
>>
>🔑*Potencia:* La realizacion del trabajo que varia con respecto al tiempo
>
>>La potencia en una masa es:
>>
>>$$P=mx^{''}x^{'}=T^{'}=m *a *v$$
>🔑*Energia disipada:*los amortiguadores disipan energia y potencia sus representaciones matematicas son:
>>
>> $$P=bx^{'2}$$

## 3.Analisis algebraico para obtener las ecuaciones de energia 

Para estos analsis se piensa que el sistema cinserva la energia,la friccion se disipa en forma de calor,los sistemas que no tiene friccion son sistemas conservativos

### 3.1Sistemas conservativos 

>🔑*sistemas conservativos:*Todas las clases de energia existentes en el sistema salen como movimientos o trabajo mecanico
>
>$$\bigtriangleup(T+U)=\bigtriangleup\omega=0$$
Para realizar el analisis es muy parecido al sistema mecanico , se formula unas ecuaciones por medio de un analisis de diagrama de cuerpo libre,despues de formular las ecuaciones se aplican las caracteristicas dinamicas y se obtiene la ecuacion(es) para el sistema

💡**Ejemplo 1:**

![image](https://github.com/user-attachments/assets/79e09adf-6ab4-4da2-93a4-dc303710dbc8)

El analisis nos da la siguiente ecuacion, teniendo encuneta las propiedades de los elementos 

$$T+U=\frac{1}{2}mx^{'2} + \frac{1}{2}k * x^{2}$$

Despues se deriva para obtener la energia total del sistema quedando:

$$\frac{1}{2}mx^{''}+kx=0$$

## 4.Conservacion movimiento Traslacional-Rotacional 

En esta parte de la clases se mostro el proceso para formular ecuaciones para sistemas que tengas movimientos rotacionales y los vuelvan movimientos translacionales 
como lo puede ser un motor moviendo unas cargas por medio de una cremallera o bandas.

Tambien se enseñaron los casos mas frecuentes y las representaciones dinamicas de lso elementos de estos sistemas, como lo es la tension,el torque,
distancia angular:

### 4.1Tension

$$T=mr^{2}\frac{d^{\theta '2} }{dt^{2}}$$

### 4.2Torque 

$$T=J\frac{d^{\theta '2} }{dt^{2}}$$

### 4.2Distancia Angular

$$\theta=\frac{y} }{r}$$

### 4.3 Analisis de sistemas 

muy parecido a los otros sistemas se hace un diagrama de cuerpo libre y se empiezan a generar las ecuaciones de modelacion algebraica
segun las propiedades y normas dadas por loe elementos, despues se agregan las caracteristicas dinamicas 

💡**Ejemplo 1:**

![image](https://github.com/user-attachments/assets/f1c6e48f-b918-450f-b922-d2717ff49cfd)

#### 4.3.1 analisis de cuerpo libre 

![image](https://github.com/user-attachments/assets/5342f65f-7d3a-44f0-b3cf-b75b68f87669)

#### 4.3.2 Analisis y Generacion de ecuaciones

$$T_{m}- T _{1} - B _{m}\frac{d\theta }{dt} = J _{m}\frac{d^{2}\theta }{dt^{2}}$$

Despues de introducir las caracteristicas dinamicas en el sistema tenemos:

$$T_{m}- Mr\frac{d^{2}y}{dt^{2}} - \frac{B _{m}}{r}\frac{dy }{dt} = \frac{J _{m}}{r}\frac{d^{2}y }{dt^{2}}$$

