# Repaso de Conocimientos Previos
## 1.Modelos Dinámicos
* En algunos campos, nos interesa representar modelos que varían con el tiempo de manera matemática para conocer sus variables en cualquier instante.

$$f(t)$$

* También nos interesa cuantificar estas variables que obtenemos en los sistemas representados

  $$\frac{df(t)}{dt}$$

## 2.Recordando Cálculo Diferencial 

>🔑 *Derivada:*  Representa la tasa de cambio instantánea de una función en un punto determinado. Matemáticamente, la derivada de una función se define como:

> Donde:
> *  $$f'(x)$$ es la derivada de $$f(x)$$
> * $$h$$ es un pequeño incremento de $$x$$

> $$f(x)$$ se define como el límite:
> $$f'(x)= lim (h→0)⁡ [(f(x+h)-f(x))/h]$$



💡**Ejemplo 1:**

$$f(x)=x^2$$

 $$\frac{df(x)}{dx}=2x$$

$$\frac{df(2)}{dx}=2x=2(2)=4$$

## 2.1 Ejercicios 

a)📚

 $$f{(x)}=x^{3}$$

$$\frac{df{(x)}}{dx}=3x^{2}$$
$$\frac{df{(1)}}{dx}=3(1)^{2}=3$$

b)📚

 $$f{(x)}=yx^{3}$$

$$\frac{df{(x)}}{dx}=3xy^{2}$$

$$\frac{df{(4)}}{dx}=3y(4)^{2}=12y$$

 ## 2.2 Modelos de Ecuaciones Diferenciales

Los modelos de ecuaciones diferenciales son representaciones matemáticas de sistemas o fenómenos del mundo real que describen cómo cambian sus variables en el tiempo.

$$a_{1}\frac{d^{2}F}{dt}+a_{2}\frac{dF}{dt}+a_{3}F=u(t)$$

* Donde F es la salida del sistema.

* U es la entrada del sistema. 

* La solución es una función derivada del sistema.

  ### 2.2.1 Características de las Ecuaciones Diferenciales

>🔑 *Ecuación Lineal Invariante en el Tiempo:* Estas ecuaciones están diseñadas para sistemas invariantes en el tiempo, es decir, aquellos que permanecen estáticos al transcurrir el tiempo. Se pueden identificar porque todas sus componentes son constantes y están elevadas a un exponente de 1.

> $$\frac{d^{2}X{(t)}}{dt^{2}}+5\frac{dx{(t)}}{dt}+10x{(t)}=0$$


>🔑 *Ecuación Lineal Variante en el Tiempo:* Estas ecuaciones se aplican en sistemas cuyo resultado no depende del tiempo, sino del valor que tengan en el instante de su aplicación. Se pueden reconocer porque algunas de sus componentes forman parte de funciones que cambian según su valor, como "sen(x)" o "cos(x)",  y todas ellas están elevadas a un exponente de 1.

> $$\frac{d^{2}X{(t)}}{dt^{2}}+(1-cos(2t))x{(t)}=0$$

>🔑 *Ecuación No Lineal Variante en el Tiempo:*  Estas ecuaciones se aplican en sistemas cuyo resultado no depende del tiempo, sino del valor que tengan en el instante de su aplicación. Se pueden reconocer porque algunas de sus componentes forman parte de funciones que cambian según su valor, como "sen(x)" o "cos(x)", y todas o algunas de ellas están elevadas a un exponente superior a 1

>$$\frac{d^{2}x{(t)}}{dt^{2}}+\frac{dx{(t)}}{dt}+x(t)+x^{3}(t)=sen(wt)$$

>🔑 *Ecuación No Lineal Invariante en el Tiempo:* Estas ecuaciones están diseñadas para sistemas invariantes en el tiempo. Se pueden identificar porque todas sus componentes son constantes y todas o algunas de ellas están elevadas a un exponente superior a 1.

>$$\frac{d^{2}x{(t)}}{dt^{2}}+(x^{2}(t)-1)\frac{dx{(t)}}{dt}+x(t)=0$$

## 3.Sistemas Lineales y No Lineales
### 3.1.Lineales 
>🔑 *sistemas Lineales:* Un sistema lineal es un modelo matemático basado en ecuaciones de primer grado y en el uso de un operador lineal. También se considera lineal cuando cumple el principio de superposición, que básicamente establece que al aplicar dos o más estímulos a un sistema, el resultado es la suma individual de sus efectos. Además, estos sistemas cumplen con la condición de proporcionalidad entre la entrada y la salida.
### 3.2.Lineales 
>🔑 *sistemas no Lineales:* Son sistemas en los que sus componentes varían de grado o incluyen operadores que pueden cambiar según su valor. Este sistema no cumple con el principio de superposición. Sin embargo, estos sistemas pueden ser linealizados en un punto donde se cumpla dicho principio.

## 4.Modelamiento y Validación 

Al realizar este proceso, es importante considerar el nivel de incertidumbre que puede tener nuestro modelo matemático. La mejor forma de hacerlo es obtener una salida en nuestro sistema teórico y compararla con los valores de nuestro sistema físico. De esta manera, podemos determinar si el nivel de incertidumbre es aceptable o no.
 ### 4.1Influencia de Parámetros 
Es una manera sencilla de entender ciertos escenarios que pueden presentarse. Dos ejemplos de ello son:

* Comportamiento sinusoidal: En este caso, podemos observar que la variable a obtener se comportará de manera sinusoidal cuando sea medida a través del tiempo.

* Decaimiento de parámetros: En este caso, podemos observar que la variable a obtener o que será observada disminuirá de manera exponencial.

* Combinación de las dos anteriores: Es una suma de las dos anteriores; la variable se mueve de manera sinusoidal y, al mismo tiempo, va disminuyendo.
   
## 5.Transformada de LaPlace

La Transformada de Laplace es un método o forma de resolver ecuaciones diferenciales mediante un cambio geométrico del dominio del tiempo al dominio de la frecuencia. Es uno de los métodos más utilizados para la solución de sistemas.

 $$x(t)-> X(s)$$

$$X(s)=\int_{0}^{inf} x(t)*e^{-st}$$

### 5.1.Transformada Inversa de LaPlace

Es una manera de regresar una ecuación diferencial que fue transformada del dominio del tiempo (t) al dominio de la frecuencia (s) nuevamente al tiempo (t),Cuando la transformada es directa, el proceso es sencillo, pero si es una combinación de diferentes funciones, es necesario descomponerla en fracciones parciales para simplificarla y facilitar su solución.

$$X(s)-> x(t)$$

### 5.1.1 Propiedades 

Nos demostraron algunas propiedades como la linealidad, el desplazamiento, el desplazamiento en s y el escalado en t .

### 5.1.2Tranformada escalon unitario 

Es una técnica utilizada para definir el segundo teorema de traslación o traslación en el tiempo. Se emplea principalmente en informática para idealizar un interruptor, haciendo que cuando t>0  represente un 1 lógico y cuando t<=0 es un 0 lógico.

### 5.1.3Tranformada funcion rampa

Es una función real que es continua y diferenciable en todo su dominio, excepto en un punto(1,1)Se utiliza en electrónica para representar sobrecorrientes. Su función representativa es:

$$L[tu(u)]=\frac{1}{s^{2}}$$

### 5.1.3Transformada de la Función Sinusoidal

Es una manera de trasladar la función sinusoidal de diferentes formas. Su transformada es:

$$L[Asen(wt)]=\frac{Aw}{(s^{2}+w^{2})}$$

### 5.1.3Transformada de una Función

$$L[f(t)]=F(s)$$

### 5.1.4Transformada de la Derivada 

$$L[f^{n}(t)]=s^{n}F(s)-s^{n-1}f(0)-...-sf^{n-1}(0)-f^{n}(0)$$

## 6.Descomposición en Fracciones Parciales 
Se identifican cuatro casos, pero en esta clase solo vimos dos de ellos. Se propusieron algunos ejercicios en clase. 

 ### 6.1.Caso 1

 En este caso, se trabaja con raíces reales y distintas. Se aplica la transformada inversa de Laplace y se descompone en fracciones parciales para resolverla. 
 
💡 **Ejemplo 1:** Obtenga la transformada inversa de:

$$G(s)=\frac{2s^{2}-4}{(s+1)(s-2)(s-3)}$$

$$\frac{2s^{2}-4}{(s+1)(s-2)(s-3)}=\frac{A}{(s+1)}+\frac{B}{(s-2)}+\frac{C}{(s-3)}$$

$$2(s^{2}-2)=A(s-2)(s-3)+B(s+1)(s-3)+C(s+1)(s-2)$$

$$A=-1/6$$ 

$$B=-4/3$$

$$C=7/2$$

$$g(t)=\frac{-1}{6}e^{-t}-\frac{4}{3}e^{2t}+\frac{7}{2}e^{3t}$$

### 6.1.1 Ejercicios

a)📚

$$F(s)=\frac{2s+7}{(s-9)(s+5)}$$


$$\frac{2s+7}{(s-9)(s+5)}=\frac{A}{(s-9)}+\frac{B}{(s+5)}$$

$$2s+7=A(s+5)+B(s-9)$$

$$A=\frac{25}{14}$$

$$A=\frac{3}{14}$$

$$f(t)=\frac{25}{14}e^{9t}+\frac{3}{14}e^{-5t}$$

b)📚

$$F(s)=\frac{s-1}{(s-2)(s-3)}$$

$$\frac{s-1}{(s-2)(s-3)}=\frac{A}{(s-2)}+\frac{B}{(s+3)}$$

$$B=2$$

$$A=-1$$

$$f(t)=-e^{2t}+2e^{3t}$$


 ### 6.2.Caso 2

 En este caso, analizamos cuando las raíces son iguales. Se tiene una transformada y se aplica su inversa, descomponiéndola en fracciones parciales con raíces iguales.

 💡 **Ejemplo 1:** Obtenga la transformada inversa de:

  $$G(s)=\frac{2s^{2}+6s+5}{(s+2)(s+1)^{2}}$$

  $$\frac{2s^{2}+6s+5}{(s+2)(s+1)^{2}}=\frac{A}{(s+2)}+\frac{B}{(s+1)}+\frac{c}{(s+1)^{2}}$$

  $$2s^{2}+6s+5=A(s+1)^{2}+B(s+2)(s+1)+C(s+2)$$

  $$A=1$$

  $$B=1$$

  $$C=1$$
 
$$g(t)=e^{-2t}+e^{-t}+te^{-t}$$

### 6.2.1 Ejercicios

a)📚

$$F(s)=\frac{s^{2}+2s+3}{(s+1)^{3}}$$

$$\frac{s^{2}+2s+3}{(s+1)^{3}}=\frac{A}{(s+1)}+\frac{B}{(s+1)^{2}}+\frac{C}{(s+1)^{3}}$$

  $$s^{2}+2s+3=A(s+1)^{3}+B(s+1)^{2}+C$$

$$A=1$$

$$B=0$$

$$C=2$$

$$f(t)=e^{-t}+t^{2}e^{-t}$$

b)📚

$$F(s)=\frac{2s^{2}+1}{(s-2)^{3}}$$

$$\frac{2s^{2}+1}{(s-2)^{3}}=\frac{A}{(s-2)}+\frac{B}{(s-2)^{2}}+\frac{C}{(s-2)^{3}}$$

$$2s^{2}+1=A(s-2)^{3}+B(s-2)^{2}+C$$

$$A=2$$

$$B=8$$

$$C=9$$

$$f(t)=2e^{t}+8te^{2t}+\frac{9t^{2}e^{2t}}{2}$$

## 7.Conclusiones 

En esta clase se hizo un repaso completo de cálculo diferencial, cálculo integral y ecuaciones diferenciales. Se recordaron métodos y pasos a seguir en dos de los diferentes casos de transformadas inversas.

## 8.Referencias 

* https://www.youtube.com/watch?v=HZZ9SFTFlyo

* https://www.youtube.com/watch?v=C3nEBf_Vgzg
