# Corrección del Parcial del Segundo Corte 
En este documento se presenta y explica el proceso correcto para la resolución del parcial correspondiente al segundo corte, según el enunciado del examen que me fue asignado.
## 1. Primer ejercicio

![WhatsApp Image 2025-05-12 at 11 36 09 PM](https://github.com/user-attachments/assets/87412fdc-b402-4f65-aaec-ada3074910d7)

### 1.1 Analisis primera masa

Como primer paso vamos hacer el diagrama de cuerpo libre de la primera masa (Normalmente es en la que actua la fuerza de entrada (u) )para ver que fuerzas actuan sobre ella

![WhatsApp Image 2025-05-12 at 11 40 01 PM](https://github.com/user-attachments/assets/c1514f99-c02b-4c70-8de7-c9eb9a1a0640)

Como podemos observar en nuestro diagrama de cuerpo libre, identificamos las fuerzas que actúan sobre la masa 1. Estas incluyen la fricción, los amortiguadores (o el rozamiento con las paredes), y la fuerza de los resortes, que se oponen al movimiento generado por la fuerza de entrada "U".
En este sistema, consideramos como positivas todas las fuerzas que se dirigen hacia abajo, y como negativas aquellas que se dirigen hacia arriba. Con base en esta convención de signos, obtenemos la siguiente ecuación de fuerzas:

$$U+F _{w1} - F _{k2} -F _{B1} -F _{B2} -F _{B3} - F _{k1} = m _{1} * a _{m1}$$

### 1.2 Analisis segunda  masa

Como segundo paso, realizamos el mismo procedimiento aplicado a la masa 1, pero ahora enfocado en la masa 2. En primer lugar, se construye el diagrama de cuerpo libre correspondiente, identificando todas 
las fuerzas que actúan sobre ella. Posteriormente, se formula la ecuación de fuerzas considerando los mismos parámetros y convenciones utilizados previamente, tales como la dirección positiva del movimiento y la acción de elementos como resortes, amortiguadores y fricción.

![WhatsApp Image 2025-05-13 at 1 04 46 AM](https://github.com/user-attachments/assets/f0253c7b-2be8-482a-af0b-5b326a8f0df4)

Con el diagrama de cuerpo libre obtenemos que la ecuacion es:

$$F _{k1}+F _{w2} -F _{B3}   = m _{2} * a _{m2}$$

### 1.3 Reemplazo de las fuerzas 

Una vez obtenidas las ecuaciones de fuerzas para ambas masas, procedemos a reemplazar las fuerzas por sus características dinámicas (como masa, constante del resorte y coeficiente de amortiguamiento). Posteriormente, relacionamos las posiciones de las masas mediante las variables 
$$y _{1(𝑡)}$$ y $$y _{2(𝑡)}$$, lo que nos permite obtener el siguiente sistema de ecuaciones diferenciales que describe el comportamiento del sistema:

1) $$U+ (m _{1} * g) - k _{2} * y _{1(𝑡)} - B _{1} * y _{1(𝑡)} ^{ ' } - B _{2} * y _{1(𝑡)} ^{ ' } - B _{3} * ( y _{1(𝑡)} ^{ ' } -  y _{2(𝑡)} ) - k _{1} * ( y _{1(𝑡)}  -  y _{2(𝑡)} ) = m _{1} * y _{1(𝑡)} ^{ '' }$$
2) $$k _{1} * ( y _{1(𝑡)}  -  y _{2(𝑡)} ) +(m _{2} * g ) - B _{3} * ( y _{1(𝑡)} ^{ ' } -  y _{2(𝑡)} )   = m _{2} * y _{2(𝑡)} ^{ '' }$$
