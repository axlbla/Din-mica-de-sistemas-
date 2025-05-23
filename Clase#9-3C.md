# Función de Transferencia

Es una representación en el dominio de Laplace que permite analizar el comportamiento de un sistema sin necesidad de resolver directamente las ecuaciones diferenciales.
Para obtenerla, se debe expresar la salida en función de la entrada, es decir, despejar la razón entre la transformada de la salida y la transformada de la entrada.

$$\frac{Y _{s}}{U _{s}}$$

Para realizar este proceso, es necesario que las condiciones iniciales del sistema sean iguales a cero $$y _{0} = 0$$ (*Esto solo se hace cuando se realiza la funcion de transferencia*).
, lo que permite aplicar la transformada de Laplace de forma simplificada.  

La función de transferencia se expresa como:

$$G _{s} = \frac{N _{s}}{D _{s}}$$

Donde:

* $$G _{s}$$ es la función de transferencia del sistema,
* $$N _{s}$$ es la transformada de Laplace de la salida,
* $$D _{s}$$ es la transformada de Laplace de la entrada.

Donde $$N _{s}$$ y $$D _{s}$$ son polinomios $$"S"$$ ,gracias a estos componentes, podemos clasificar las funciones de transferencia según sus ceros y polos.
Para ello, utilizamos un método que se define de la siguiente manera:

-Si denominamos $$n$$ al grado del numerador. 

-si denominamos  $$m$$ al grado del denominador.

Gracias a esto, también podemos clasificar los diferentes tipos de sistemas que existen, según su comportamiento y características dinámicas.

## 1. Clasificación de Sistemas

-Si $$n>m$$ es un sistema impropio.

>🔑 *Sistema Impropio:* Son sistemas en los que el grado del numerador es mayor que el del denominador en la función de transferencia.Este tipo de sistemas, también conocidos como no físicamente realizables, suelen asociarse teóricamente a sistemas que generan energía, lo cual no ocurre en sistemas reales pasivos.Por esta razón, los sistemas impropios son poco comunes y, en la práctica, suelen considerarse no realizables.

 -Si $$m>n$$ es un sistema Estrictamente Propio.

 >🔑 *Sistema Estrictamente Propio:* Son sistemas en los que el grado del denominador es mayor que el del numerador en la función de transferencia.Estos sistemas representan comportamientos en los que la salida responde a una entrada de manera física y realista, es decir, requieren tiempo para procesar la señal antes de producir una salida.
Son los más comunes en la naturaleza y en los sistemas físicos, ya que modelan adecuadamente fenómenos donde no puede haber una respuesta instantánea.

-Si $$m=n$$ es un sistema Bipropio.

>🔑 *Sistema Bipropio:* Son sistemas en los que el grado del numerador y del denominador son iguales en la función de transferencia.Estos sistemas suelen representar una respuesta instantánea a cambios en la señal o energía de entrada.
Aunque existen teóricamente, son poco comunes en el análisis práctico de sistemas físicos debido a las limitaciones reales de procesamiento y respuesta instantánea.

💡**Ejemplo 1:**  Clasificación de Sistemas

$$G _{s} = s ^{2} + 1$$  $$n = 2$$  $$m=0$$  $$n>m$$

Por ende es un sistema impropio 


## 2. Ceros de la Función de Transferencia

Para encontrar los valores de los ceros de una función de transferencia, se deben tener en cuenta dos aspectos importantes:

*Los valores de $$s$$ que hacen que el polinomio sea igual a cero, es decir, que satisfacen la ecuación $N _{s} = 0$$.

*Estos valores pueden ser reales o complejos.

$$G _{s} = \frac{N _{s}}{D _{s}}= 0$$

💡**Ejemplo 1:**  Ceros de la Función de Transferencia

$$G _{s} = \frac{Y _{s}}{U _{s}}= \frac{3s-1}{s ^{2} +3s +2} = \frac{N _{s}}{D _{s}}$$

$$Y _{s}= 0$$ $$3s-1=0$$ $$s= \frac{1}{3}$$

### 2.1. Graficacion de los ceros de la funcion de transferencia 

Para graficar los ceros es tan facil como ubicarlos en un plano cartesiano en los que el eje $$x$$ va ha ser los numeros reales $$(R)$$ y el eje $$y$$ es son los numeros imaginarios $$(I)$$.

Cada cero se representa como un círculo que marca el valor de $$s$$ que hace cero al polinomio del numerador de la función de transferencia.

💡**Ejemplo 2:**  Ceros de la Función de Transferencia

Siguiendo el ejemplo anterior obtenemos 

![cero_1_3](https://github.com/user-attachments/assets/2a68b3d2-50df-4c08-b43f-a139bd9e7b4b)



