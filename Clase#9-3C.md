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

- Sí denominamos $$n$$ al grado del numerador. 

- sí denominamos  $$m$$ al grado del denominador.

Gracias a esto, también podemos clasificar los diferentes tipos de sistemas que existen, según su comportamiento y características dinámicas.

## 1. Clasificación de Sistemas

- Sí $$n>m$$ es un sistema impropio.

>🔑 *Sistema Impropio:* Son sistemas en los que el grado del numerador es mayor que el del denominador en la función de transferencia.Este tipo de sistemas, también conocidos como no físicamente realizables, suelen asociarse teóricamente a sistemas que generan energía, lo cual no ocurre en sistemas reales pasivos.Por esta razón, los sistemas impropios son poco comunes y, en la práctica, suelen considerarse no realizables.

 - Sí $$m>n$$ es un sistema Estrictamente Propio.

 >🔑 *Sistema Estrictamente Propio:* Son sistemas en los que el grado del denominador es mayor que el del numerador en la función de transferencia.Estos sistemas representan comportamientos en los que la salida responde a una entrada de manera física y realista, es decir, requieren tiempo para procesar la señal antes de producir una salida.
Son los más comunes en la naturaleza y en los sistemas físicos, ya que modelan adecuadamente fenómenos donde no puede haber una respuesta instantánea.

- Sí $$m=n$$ es un sistema Bipropio.

>🔑 *Sistema Bipropio:* Son sistemas en los que el grado del numerador y del denominador son iguales en la función de transferencia.Estos sistemas suelen representar una respuesta instantánea a cambios en la señal o energía de entrada.
Aunque existen teóricamente, son poco comunes en el análisis práctico de sistemas físicos debido a las limitaciones reales de procesamiento y respuesta instantánea.

💡**Ejemplo 1:**  Clasificación de Sistemas

$$G _{s} = s ^{2} + 1$$  $$n = 2$$  $$m=0$$  $$n>m$$

Por ende es un sistema impropio.


## 2. Ceros de la Función de Transferencia

Para encontrar los valores de los ceros de una función de transferencia, se deben tener en cuenta dos aspectos importantes:

* Los valores de $$s$$ que hacen que el polinomio sea igual a cero, es decir, que satisfacen la ecuación $N _{s} = 0$$.

* Estos valores pueden ser reales o complejos.

$$G _{s} = \frac{N _{s}}{D _{s}}= 0$$

💡**Ejemplo 1:**  Ceros de la Función de Transferencia

$$G _{s} = \frac{Y _{s}}{U _{s}}= \frac{3s-1}{s ^{2} +3s +2} = \frac{N _{s}}{D _{s}}$$

$$Y _{s}= 0$$ $$3s-1=0$$ $$s= \frac{1}{3}$$

### 2.1. Graficación de los ceros de la función de transferencia 

Para graficar los ceros, es tan fácil como ubicarlos en un plano cartesiano en el que el eje $$x$$ va a ser los números reales  $$(R)$$ y el eje $$y$$ serán los números imaginarios $$(I)$$.

Cada cero se representa como un círculo que indica el valor de $$s$$ que anula el polinomio del numerador de la función de transferencia.

💡**Ejemplo 2:**  Ceros de la Función de Transferencia

Siguiendo el ejemplo anterior, obtenemos:

![cero_1_3](https://github.com/user-attachments/assets/2a68b3d2-50df-4c08-b43f-a139bd9e7b4b)


## 3. Polos de la Función de Transferencia

Para encontrar los polos de una función de transferencia, se deben tener en cuenta dos aspectos importantes, al igual que con los ceros en las funciones. 

* Sí  $$D _{s}$$ tiene valores donde $$s$$ de 0.
* Estos valores pueden ser Reales o Complejos.

$$G _{s} = \frac{N _{s}}{D _{s}}= Indeterminado $$

💡**Ejemplo 1:**  Polos de la Función de Transferencia

$$\frac{3s-1}{s ^{2} + 3s +2}$$

$$D _{s}=s ^{2} + 3s +2 = (s+1)(s+2)$$

* Primer polo de la función. 

$$s+1=0$$

$$s=-1$$

* Segundo polo de la función.

$$s+2=0$$

$$s=-2$$

### 3.1. Clasificación de los polos 

En los polos de una función de transferencia, podemos encontrar tres tipos de polos:

* Iguales y repetidos.

* Imaginarios conjugados. 

* Reales y diferentes.

![Captura de pantalla 2025-05-25 213459](https://github.com/user-attachments/assets/fece83b4-85e5-4a74-ada1-eb0d0edecb46)

## 3.2  Graficación de los polos de la función de transferencia 

Para graficar los polos, es tan fácil como ubicarlos en un plano cartesiano en el que el eje $$x$$ va a ser los números reales  $$(R)$$ y el eje $$y$$ serán los números imaginarios $$(I)$$.

Cada polo se representa como una "X" que indica el valor de $$s$$ que anula el polinomio del denominador de la función de transferencia.

💡**Ejemplo 2:**  Polos de la Función de Transferencia

Siguiendo el ejemplo anterior, obtenemos:

$$s=-1$$

$$s=-2$$

![Captura de pantalla 2025-05-25 213459](https://github.com/user-attachments/assets/cc643298-6198-4308-92f7-cad94a0049f6)

## 4. Teorema del valor Final 

Este teorema nos ayuda a definir, por medio de los límites, los posibles valores finales que va a tomar la función cuando llegue a su estado estacionario. Para realizar este análisis es importante tener en cuenta que el error en estado estacionario corresponde a $$t=\infty$$.

$$ \ lim_{ t \to \infty } f _ {(t)} = \ lim _{s \to 0 } F _ {(s)}$$

$$G _{(s)}=\frac{Y _{(s)}}{U _{(s)}}$$

Para realizar este tipo de análisis, tenemos que usar señales de entrada características, para conocer las características de los sistemas según cómo reaccionan a las mismas, tales como:

>🔑 *Entrada escalon :*  Se utiliza para saber que tan rapido es el sitemas en cambiar de estado y su señal caracteristica es:
>
> $$L [ u _{t}  ]= \frac{A}{s}$$
>
> Su gráfica característica es:
>
> ![Escalon](https://github.com/user-attachments/assets/e5feed80-2a10-47af-8fea-ba6ff9789691)

>🔑 *Entrada Rampa :* Se utiliza para evaluar si el sistema es capaz de seguir un cambio constante al aplicar una señal. Su señal caracteristica es:
>
> $$L [ x _{t}  ]= \frac{A}{s ^{2}}$$
>
> Su gráfica característica es:
>
>![rampa](https://github.com/user-attachments/assets/372faaf4-3bf6-439a-b393-cff5d2860fd2)

>🔑 *Entrada Parabola :* Se utiliza para entender cómo se comporta el sistema al aplicar una aceleración o desaceleración en el mismo. Su señal característica es:
>
> $$L [ x _{t}  ]= \frac{A}{s ^{3}}$$
>
>Su gráfica característica es:
>
>![parabola](https://github.com/user-attachments/assets/e09d2396-f0a8-4a3b-811b-b8db4123e288)
>

💡**Ejemplo 1:**  Teorema del valor Final 

$$Y _{(s)}= \frac{4* U _{s}}{5s+1}$$

* Entrada a analizar: Señal Escalon

$$L [ u _{t}  ]= \frac{1}{s}$$

* Reemplazando la entrada en la función de transferencia: 

$$Y _{(s)}= \frac{4* \frac{1}{s} }{5s+1}$$

* Aplicando el analisis del Teorema del valor final en la función de transferencia: 

$$\ lim _{s \to 0 } s Y _{(s)}$$

$$\ lim _{s \to 0 } s (\frac{4* \frac{1}{s} }{5s+1})$$

* Obtenemos que el valor final del sistema, en su estado estacionario, es:

$$\ lim _{s \to 0 } (\frac{4}{5s+1}) =4$$

## 5. Conclusión

En conclusión, en esta clase aprendimos a identificar características de los sistemas por medio del análisis de las funciones de transferencia, tales como:

* Tipos de funciones de transferencia.
* Ceros de las funciones de transferencia.
* Polos de las funciones de transferencia.
* El grado de la función de transferencia.
* Comportamiento según la entrada aplicada al sistema.

Estas son algunas de las cosas que ya podemos identificar gracias al análisis enseñado en esta clase. También aprendimos a graficar los valores que toma $$𝑠$$ para evaluar los ceros de las funciones, así como los valores que toma $$𝑠$$ para identificar los polos de las funciones.

## 6. Ejercicios adicionales 
* Identifique en las siguientes funciones sus ceros, polos, el tipo de función y su valor final utilizando una entrada escalón:
💡**Ejemplo 1:**

$$G _{s}= \frac{8}{s ^{3}+6 s ^{2} + 11s + 6}$$
* Ceros de la funcion:
R/ No presenta ceros
* Polos de la funcion
$$
  
