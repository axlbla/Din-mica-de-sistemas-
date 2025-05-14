# 1. Corrección del Parcial del Segundo Corte 
En este documento se presenta y explica el proceso correcto para la resolución del parcial correspondiente al segundo corte, según el enunciado del examen que me fue asignado.

## 1.1 Primer ejercicio

![WhatsApp Image 2025-05-12 at 11 36 09 PM](https://github.com/user-attachments/assets/87412fdc-b402-4f65-aaec-ada3074910d7)

### 1.1.1 Analisis primera masa

Como primer paso vamos hacer el diagrama de cuerpo libre de la primera masa (Normalmente es en la que actua la fuerza de entrada (u) )para ver que fuerzas actuan sobre ella

![WhatsApp Image 2025-05-12 at 11 40 01 PM](https://github.com/user-attachments/assets/c1514f99-c02b-4c70-8de7-c9eb9a1a0640)

Como podemos observar en nuestro diagrama de cuerpo libre, identificamos las fuerzas que actúan sobre la masa 1. Estas incluyen la fricción, los amortiguadores (o el rozamiento con las paredes), y la fuerza de los resortes, que se oponen al movimiento generado por la fuerza de entrada "U".
En este sistema, consideramos como positivas todas las fuerzas que se dirigen hacia abajo, y como negativas aquellas que se dirigen hacia arriba. Con base en esta convención de signos, obtenemos la siguiente ecuación de fuerzas:

$$U+F _{w1} - F _{k2} -F _{B1} -F _{B2} -F _{B3} - F _{k1} = m _{1} * a _{m1}$$

### 1.1.2 Analisis segunda  masa

Como segundo paso, realizamos el mismo procedimiento aplicado a la masa 1, pero ahora enfocado en la masa 2. En primer lugar, se construye el diagrama de cuerpo libre correspondiente, identificando todas 
las fuerzas que actúan sobre ella. Posteriormente, se formula la ecuación de fuerzas considerando los mismos parámetros y convenciones utilizados previamente, tales como la dirección positiva del movimiento y la acción de elementos como resortes, amortiguadores y fricción.

![WhatsApp Image 2025-05-13 at 1 04 46 AM](https://github.com/user-attachments/assets/f0253c7b-2be8-482a-af0b-5b326a8f0df4)

Con el diagrama de cuerpo libre obtenemos que la ecuacion es:

$$F _{k1}+F _{w2} -F _{B3}   = m _{2} * a _{m2}$$

### 1.1.3 Reemplazo de las fuerzas 

Una vez obtenidas las ecuaciones de fuerzas para ambas masas, procedemos a reemplazar las fuerzas por sus características dinámicas (como masa, constante del resorte y coeficiente de amortiguamiento). Posteriormente, relacionamos las posiciones de las masas mediante las variables 
$$y _{1(𝑡)}$$ y $$y _{2(𝑡)}$$, lo que nos permite obtener el siguiente sistema de ecuaciones diferenciales que describe el comportamiento del sistema:

1) $$U+ (m _{1} * g) - k _{2} * y _{1(𝑡)} - B _{1} * y _{1(𝑡)} ^{ ' } - B _{2} * y _{1(𝑡)} ^{ ' } - B _{3} * ( y _{1(𝑡)} ^{ ' } -  y _{2(𝑡)} ^{ ' } ) - k _{1} * ( y _{1(𝑡)}  -  y _{2(𝑡)}  ) = m _{1} * y _{1(𝑡)} ^{ '' }$$
2) $$k _{1} * ( y _{1(𝑡)}  -  y _{2(𝑡)} ) +(m _{2} * g ) - B _{3} * ( y _{1(𝑡)} ^{ ' } -  y _{2(𝑡)} ^{ ' } )   = m _{2} * y _{2(𝑡)} ^{ '' }$$

Como resultado final del análisis, obtenemos dos ecuaciones diferenciales de segundo orden que representan el comportamiento dinámico del sistema mecánico Resorte–Amortiguador–Masa. Estas ecuaciones describen la interacción entre las dos masas a través de los elementos elásticos (resortes) y disipativos (amortiguadores), permitiendo modelar con precisión la respuesta del sistema ante una fuerza de entrada.

## 1.2. Segundo ejercicio

![WhatsApp Image 2025-05-13 at 9 04 21 PM](https://github.com/user-attachments/assets/8993096b-cc07-486f-a7ff-4dbb4d271df8)

### 1.2.1 Análisis del Circuito

Como primer paso, se define el tipo de análisis que se utilizará para estudiar el circuito eléctrico. En este caso, se opta por el método de nodos, ya que permite simplificar el procedimiento y facilita la obtención de la ecuación que representa el comportamiento del circuito.

Antes de iniciar con el análisis, se establecen algunas convenciones:

1) El voltaje en la resistencia de 50 ohmios se representará como $$y _{t}$$.
2) Todas las corrientes se considerarán saliendo del nodo con signo negativo, excepto la corriente $$I _{1}$$, que se tomará con signo positivo.

Estas definiciones permiten mantener coherencia en la formulación de las ecuaciones nodales y en la interpretación de los resultados.

![WhatsApp Image 2025-05-13 at 10 05 31 PM](https://github.com/user-attachments/assets/4ef6e009-d5b5-40ac-8633-3c8a511a1821)

Teniendo en cuenta todo lo descrito anteriormente y aplicando el análisis al circuito mediante el método de nodos, se obtiene la siguiente ecuación (o conjunto de ecuaciones) que representa el comportamiento eléctrico del sistema:

$$I _{1} - I _{2} - I _{3}=0$$

Reemplazando las corrientes en términos de voltajes e impedancias, obtenemos:

$$I _{1} - 0.2 \frac{d(v _{t})}{d _{t}}  - \frac{y _{t}}{50}=0$$

Se realiza un análisis de igualdad de valores con respecto de $$y _{t}$$ 

$$y _{t} = 4 \frac{d(v _{t})}{d _{t}} + \frac{1}{0,2} \int i _{t} * dt$$

Ya para acabar, se realiza un análisis de la corriente $$I _{1}$$ obteniendo:

$$-e _{t} = 2 \frac{ i _{1(t)}}{d _ {t}} + 200i _{1(t)}+ 4 \frac{d(v _{t})}{d _{t}} + \frac{1}{0,2} \int i _{t} * d _{t}$$

Despejando $$I _{1}$$ obtenemos:

$$\frac{ -(e _{t} + 2 \frac{ i _{1(t)}}{d _ {t}} + 4 \frac{d(v _{t})}{d _{t}} + \frac{1}{0,2} \int ( i _{t} * d _{t}) }{200}$$

Por último, reemplazamos la ecuación obtenida en la ecuación nodal para obtener la ecuación del sistema en términos de la entrada y la salida, obteniendo:

$$\frac{ -(e _{t} + 2 \frac{ i _{1(t)}}{d _ {t}} + 4 \frac{d(v _{t})}{d _{t}} + \frac{1}{0,2} \int ( i _{t} * d _{t}) }{200} -  0.2 \frac{d(v _{t})}{d _{t}}  - \frac{y _{t}}{50}=0$$

Siendo esta última la ecuación del sistema obtenida mediante el análisis nodal.

# 2. Conclusión

En conclusión, se realizaron ejercicios de análisis mecánico y eléctrico, poniendo en práctica los conocimientos adquiridos durante el segundo corte. Este enfoque permitió aplicar las técnicas de modelado y análisis, tanto en el ámbito físico como en el eléctrico, para obtener las ecuaciones que describen el comportamiento del sistema. Estos ejercicios refuerzan la comprensión de los conceptos estudiados.
