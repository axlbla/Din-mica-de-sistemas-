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

# 2.1 Ejercicios 

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

>🔑 *sistemas no Lineales:* son  sistemas en las que sus componentes varian de grado o se encuentran operadores que pueden cambiar segun su valor este sistema no cumple con el principio de superposicion,estos sitemas se linealizan a un punto en donde se cumpla el principio de superposicon.

## 4.Modelamiento y Validacion 







