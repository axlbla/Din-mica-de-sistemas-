# Repaso de Conocimientos Previos
## 1.Modelos Dinamicos 
* En algunos campos no sinteresa representar modelos que varian con el tiempo de manera matematica para conocer sus variables en cualquier instante.

$$f(t)$$

* Tambien nos es de interes cuantificar estas variables que obtenemos en los sitemas reprensentados.

  $$\frac{df(t)}{dt}$$

## 2.Recordando calculo diferencial 

>🔑 *Derivada:*  representa la tasa de cambio instantánea de una función en un punto determinado. Matemáticamente, la derivada de una función

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

 ## 2.2 Modelos de ecuacion diferenciales 

Los modelos de ecuaciones diferenciales son representaciones matemáticas de sistemas o fenómenos del mundo real.

$$a_{1}\frac{d^{2}F}{dt}+a_{2}\frac{dF}{dt}+a_{3}F=u(t)$$

* Donde F es la salida del sistema

* U es la entrada del sistema 

* La solucion es una funcion derivada del sistema

  ### 2.2.1 Caracteristicas de las ecuaciones diferenciales

>🔑 *Ecuacion Lineal Invariante en el tiempo:* Estas ecuaciones estan hechas para sistemas invariantes en el tiempo , o que permanecen estaticos al pasar el tiempo , se pueden identificar por que todas sus componentes son constantes y todas ellas estan elevadas a un exponente 1:

> $$\frac{d^{2}X{(t)}}{dt^{2}}+5\frac{dx{(t)}}{dt}+10x{(t)}=0$$


>🔑 *Ecuacion Lineal Variante En El tiempo:* Estas ecuacions se aplican en sistemas en los cuales su resultado no depende del tiempo si no de el valor que tenga en el instante de la aplicacion de la misma, se pueden reconocer por que algunas de sus componentes hacen parte de funciones que cambian segun su valor como "sen(x)" o "cos(x)" y todas ellas estan elevadas a un exponente 1:

> $$\frac{d^{2}X{(t)}}{dt^{2}}+(1-cos(2t))x{(t)}=0$$

>🔑 *Ecuacion No Lineal Variante En El Tiempo:*  Estas ecuacions se aplican en sistemas en los cuales su resultado no depende del tiempo si no de el valor que tenga en el instante de la aplicacion de la misma, se pueden reconocer por que algunas de sus componentes hacen parte de funciones que cambian segun su valor como "sen(x)" o "cos(x)" y todas o algunas ellas estan elevadas a un exponente superior de 1:

>$$\frac{d^{2}x{(t)}}{dt^{2}}+\frac{dx{(t)}}{dt}+x(t)+x^{3}(t)=sen(wt)$$

>🔑 *Ecuacion no Lineal Invariante en el tiempo:* Estas ecuaciones estan hechas para sistemas invariantes en el tiempo ,  se pueden identificar por que todas sus componentes son constantes y todas o algunas ellas estan elevadas a un exponente superior de 1:

>$$\frac{d^{2}x{(t)}}{dt^{2}}+(x^{2}(t)-1)\frac{dx{(t)}}{dt}+x(t)=0$$

## 3.Sistemas Lineales y No lineales 
### 3.1.Lineales 
>🔑 *sistemas Lineales:* Un sistema lineal es un modelo matemático que se basa en ecuaciones de primer grado y en el uso de un operador lineal.Tambien se concidera lineal cuando se cumple el principio de superposicion basicamente nos dice que al aplicar dos o mas estiumulos a un sistema nuestro resultado es la suma individul de las mismas.estos tambien cumplen con la condicion de porporcionalidad entre entrada y salida.
### 3.2.Lineales 
>🔑 *sistemas no Lineales:* son  sistemas en las que sus componentes varian de grado o se encuentran operadores que pueden cambiar segun su valor este sistema no cumple con el principio de superposicion,estos sitemas se linealizan a un punto en donde se cumpla el principio de superposicon.

## 4.Modelamiento y Validacion 

Al realizarce este proceso se tiene que tener el nivel de incertidumbre que puede llegar a tener nuestro modelo matematico la mejor forma para hacer esto es el tener obtener una salida en nuestro sistema teorico y compararlo con los valores de nuestro sistema fisico, asi podemos mirar si el nivel de incertidumbre es aceptable o no.
 ### 4.1Influencia de parametros 
Es una manera sencilla de entender ciertos escenarios que se pueden llegar a ver o obtener dos ejemplos de ellos son 

* Comportamiento sinusoidal: En este podemos ver que la variable a obtener se va comportar de manera sinusoidal al ser medida a traves del tiempo

* Decaimiento de parametros: en este podemos ver que la variable a obtener o que va ha ser observada va a disminuir de manera exponencial 

* Combinacion de las dos anteriores: Esta es una suma de las dos anterioses , se mueve de manera sinusoidal y al tiempo va disminuyendo
   
## 5.Transformada de LaPlace

La Transformada de LaPlace es un metodo o forma de resolver ecuaciones diferenciales , por medio de un cambio deometrico del dominio del tiempo hacia el dominio de la frecuencia, de los metodos mas usados para la solucion de sistemas.

 $$x(t)-> X(s)$$

$$X(s)=\int_{0}^{inf} x(t)*e^{-st}$$

### 5.1.Transformada Inversa de LaPlace

Es una manera de devolver una ecuacion diferencial que se paso de respecto al tiempo (t) a la frecuencia (s) devuelta al tiempo (t), cuando estas son directas son muy sencillas, pero si son una fusion de diferentes funciones se tiene que llevar a fracciones parciales para ser simplificadas y poderse solucionar de manera mas sencilla.

$$X(s)-> x(t)$$

### 5.1.1 Propiedades 

nos demostraron algunas propiedades como la lidealidad , el despalazamiento , desplazamiendto en s y el escalado en t

### 5.1.2Tranformada escalon unitario 

es una técnica que se utiliza para definir el segundo teorema de traslación o traslación en el tiempo, es utilizada principal mente en informatica para idealizar un interruptor , haceidno que cuando t>o representa un 1 logico y cuando t<=0 es un 0 logico.

### 5.1.3Tranformada funcion rampa

es una función real que es continua y diferenciable en todo su dominio, excepto en un punto (1,1) , es usada en electronica  para sobre corrientes, su funcion representativa es:

$$L[tu(u)]=\frac{1}{s^{2}}$$

### 5.1.3Tranformada funcion senosiodal

es una manera de trasladar la funcio seinusoidal de diferentes maneras su transformada es: 

$$L[Asen(wt)]=\frac{Aw}{(s^{2}+w^{2})}$$

### 5.1.3Tranformada de una funcion 

$$L[f(t)]=F(s)$$

### 5.1.4Tranformada de una funcion 

$$L[f^{n}(t)]=s^{n}F(s)-s^{n-1}f(0)-...-sf^{n-1}(0)-f^{n}(0)$$

## 6.Descomposicion en fracciones parciales 
 se identifican 4 casos , pero en esta clase solo vimos dos de ellos ,se proponen unos ejercicios en clases 

 ### 6.1.Caso 1

 en este caso se trabaja con raices reales y distintas , se tiene una transformada inversa de laPlace y se lleva a fracciones parciales para ser resuelta 
 
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

 En este caso vemos cuando son raices iguales, se tiene una transfomada y se aplica su inversa llevandose a fracciones parciales con raices iguales:

 💡 **Ejemplo 1:** Obtenga la transformada inversa de:
 
