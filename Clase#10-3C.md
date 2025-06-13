# Modelamiento de sistemas con diagramas de bloques

Método para modelar sistemas complejos o compuestos por diferentes subsistemas de manera más sencilla, por medio de funciones de transferencia, señales de entrada y salida. Nos apoyamos en un método llamado diagrama de bloques. 

## 1.Sistemas conocidos 

Para empezar el modelamiento de un sistema por medio de diagramas de bloques, se inicia con el análisis del sistema, realizando una partición del mismo. Con el siguiente ejemplo, mostraremos cómo hacer el análisis en cada caso que se presente.

💡**Ejemplo 1:** Vamos a hacer el análisis de un solenoide por medio del modelamiento con diagramas de bloques.

![image](https://github.com/user-attachments/assets/71628b30-3782-4749-9208-864e3e6f1a4e)


### 1.1.Sistemas eléctricos

Método para el análisis de sistemas eléctricos:

💡**Ejemplo 1:** Se realiza el analisis de un solenoide haciendo primero en analisis electrico del sistema.

![WhatsApp Image 2025-06-12 at 9 40 47 AM](https://github.com/user-attachments/assets/ffc4dfe7-dd0b-4e4a-9bcf-a3177dd17156)

Primero, hacemos un análisis eléctrico utilizando el método de mallas, del cual obtenemos:

$$L\frac{\mathrm{d}i }{\mathrm{d} t}+Ri=V _{(t)}$$

Aplicando la transformada de Laplace y despejando la función de transferencia, obtenemos: 

$$\frac{I _{(s)}}{ V _{(S)}} = \frac{1}{Ls+R}$$

### 1.2.Sistemas de transformación de energía

Son sistemas que se encargan de transformar una energía entrante en otro tipo de energía, ya sea mecánica, eléctrica o rotacional. Normalmente, se representan mediante constantes o relaciones proporcionales.

💡**Ejemplo 1:** Siguiendo con el ejemplo anterior, tenemos el análisis del sistema transductor.

* Relación eléctrica con la mecánica, donde tenemos que:

  $$f _{(s)} = k _{s} * i$$

Donde tenemos que $$k _{s}$$ es una constante. Aplicando la transformada de Laplace y obteniendo la función de transferencia, se obtiene que:

$$\frac{F _{(s)} }{I _{(s)}} = K _{s}$$

### 1.3.Sistemas mecánicos

Método para el análisis de sistemas mecánicos: muy parecido al análisis clásico, se plantean las ecuaciones del sistema, pero ahora se generan funciones de transferencia.

💡**Ejemplo 1:** Siguiendo con el ejemplo anterior, hacemos el análisis mecánico de los solenoides.

![WhatsApp Image 2025-06-12 at 9 41 02 AM](https://github.com/user-attachments/assets/44391c5f-444e-4df4-836a-6a654a060473)

Haciendo el análisis mecánico, obtenemos la siguiente ecuación diferencial:

$$f _{(t)} - kx-bx^{'}= mx^{''}$$

Aplicando la transformada de Laplace y expresando en términos de la función de transferencia, obtenemos que:

$$\frac{X _{(s)}}{F _{(s)}} = \frac{1}{ms ^{2}+ bs + k}$$

##  2.Representación de bloques 

Para representar un sistema en diagramas de bloques, solo se deben tener en cuenta dos cosas: la primera es la función de transferencia y la segunda, las señales de entrada y salida.

💡**Ejemplo 1:** Siguiendo con el ejemplo anterior, hacemos la representación del diagrama de bloques del solenoide.

![image](https://github.com/user-attachments/assets/98524473-8481-4955-906b-9f20fcfd464d)

Como podemos apreciar, la representación nos indica qué variable nos va a entregar cada uno de los subsistemas, así como también la variable de salida que nos entrega el sistema. En este caso, se obtiene un movimiento lineal cuando se aplica un voltaje.

## 3.Modelamiento de sistemas más comunes

En esta parte de la clase nos enseñaron el modelamiento de un motor DC de dos formas, utilizando el mismo método de modelamiento con diagramas de bloques.

![image](https://github.com/user-attachments/assets/9b5ce080-2660-44d3-9cb0-1b8931b1114b)

Los dos métodos para analizar un motor DC son:

* Corriente de campo
  
* Corriente de armadura

En estos apuntes veremos un resumen de cada método y sus resultados.

### 3.1.Corriente de Campo

#### 3.1.1.Análisis eléctrico del motor 

Para este análisis, se aplica el método de mallas, pero se hace la suposición de que la corriente de armadura es constante.

![image](https://github.com/user-attachments/assets/fe398716-ce0e-4ccd-a950-377f012f4cd1)

Después de hacer el análisis, obtenemos que:

$$\frac{I _{(s)}}{ V _{(S)}} = \frac{1}{L _{(c)}s+R _{(c)}}$$


#### 3.1.2.Análisis electromecánico (subsistema de transformación de energía)

Para este análisis, se deben tener en cuenta varias constantes e igualdades de transformación, tales como:

* El flujo en el entrehierro es proporcional a la corriente de campo.
  
$$\phi = k _{c} i _{c}$$

* El torque desarrollado es proporcional al flujo y a la corriente de armadura. En esta relación, todas las constantes $$(k _{c} i _{c} k _{a})$$ se combinan en una sola constante $$K _{m}$$ así obtenemos:

$$T _{m}= (k _{m}) I _{c (s)}$$
  
* El torque aplicado a la carga es el generado por el motor menos el efecto de la inercia de la carga.

$$T _{c(s)}= T _{m(s)} - T _{p(s)}$$

![image](https://github.com/user-attachments/assets/b4e3324d-612f-4dbc-82d1-249b03c7ab5b)

#### 3.1.3.Análisis mecánico de la carga y el torque

En este sistema se realiza un análisis mecánico teniendo en cuenta la carga, los momentos de inercia y el torque del motor. 

![image](https://github.com/user-attachments/assets/c3f6d285-72e1-46a4-a3b5-d3f13909ba0b)

* Obtenemos la ecuación mecánica.

$$J \frac{d^2 \theta  }{d t^2} + b\frac{\mathrm{d} \theta  }{\mathrm{d} t} + k\theta  = \tau _{(t)}$$

Al obtener la función de transferencia, tenemos que:

$$\frac{\theta _{s}}{T _{c(s)}} = \frac{1}{(js ^{2} + bs)}$$

#### 3.1.4.Representación de diagramas de bloques 

Como penúltimo paso, vamos a reemplazar en las ecuaciones obtenidas en el sistema de transformación, para así empezar el análisis de los diagramas de bloques, obteniendo:

$$\theta _{s} = \frac{K _{m}}{(L _{(c)}s +R _{(c)})(js ^{2} + bs)} - T _{p(s)}\frac{1}{(js ^{2} + bs)}$$

Ya por último, hacemos la representación de los diagramas de bloques, obteniendo: 

![image](https://github.com/user-attachments/assets/4923b3b7-6e8c-4129-ab30-9d472321fde1)

### 3.1.Corriente de Armadura

#### 3.2.1.Análisis eléctrico del motor

Para este análisis, se utiliza el método de mallas, pero se hace la suposición de que la corriente de campo es constante.

![image](https://github.com/user-attachments/assets/1567eea7-8ba4-4477-bca2-0ae54717ec20)

Después de hacer el análisis, obtenemos que:

$$\frac{I _{(s)}}{ V _{(S)}} = \frac{1}{L _{(a)}s+R _{(a)}}$$


#### 3.2.2.Análisis electromecánico (subsistema de transformación de energía)

Para este análisis se deben tener en cuenta varias constantes e igualdades de transformación, tales como:

* La corriente de armadura se relaciona con el voltaje aplicado a la armadura. En este análisis se relacionan todas las constantes $$(k _{c} i _{c} k _{a})$$ combinándose en una sola constante $$K _{m}$$. Así, obtenemos:

$$T _{m}= (k _{m}) I _{a (s)}$$

* Se realiza una relación entre los voltajes y los torques, obteniendo:

$$V _{a(s)}= L _{(a)}s+R _{(a)}I _{a (s)} + V _{b(s)}$$

* El voltaje inducido en la armadura es proporcional a la velocidad angular del eje:

$$V _{b(s)}= k _{b} w _{s}$$

* Al reemplazar en las ecuaciones, se obtiene:

$$I _{(s)}= \frac{V _{a(s)}-k _{b} w _{s}}{ L _{(a)}s + R _{(a)}}$$

![image](https://github.com/user-attachments/assets/899ab540-e4ee-45e2-bd7e-db63988d29f1)

#### 3.2.3.Análisis mecánico de la carga y el torque 

* El torque aplicado a la carga es el generado por el motor menos el efecto de la inercia de la carga.

  $$T _{c(s)}= T _{m(s)} - T _{p(s)}$$

* En este sistema se realiza el mismo análisis mecánico que en el método anterior, teniendo en cuenta la carga, los momentos de inercia y el torque del motor. 

$$\frac{\theta _{s}}{T _{c(s)}} = \frac{1}{(js ^{2} + bs)}$$

![image](https://github.com/user-attachments/assets/ddab7660-6470-4531-ac13-77e65646f2b4)


#### 3.1.4.Representación de diagramas de bloques 

Ya por último, hacemos la representación de diagramas de bloques, obteniendo:

![image](https://github.com/user-attachments/assets/bfcbe3f9-40b8-4f4d-9fbd-7e5bfbfedc3a)

## 4.Relaciones de componentes en sistemas 

Son relaciones de constantes dinámicas para realizar la transformación de energía en los sistemas dinámicos. De estas, hay mecánicas, eléctricas, hidráulicas, etc.

### 4.1.Engranajes,Poleas y cremallleras 

Son dispositivos mecánicos que transmiten la energía desde una parte del sistema a otra.

![image](https://github.com/user-attachments/assets/7d957026-f4b2-44c0-8fef-90bd92e34a6b)

La representación en diagramas de bloques sería una constante por la cual se multiplica. 

![image](https://github.com/user-attachments/assets/081cb0b5-79ab-4291-8932-f043fc24a6b1)

En estos mismos sistemas, es muy común el uso de cremalleras, que transforman el movimiento rotacional en movimiento lineal, obteniendo:

![image](https://github.com/user-attachments/assets/188d5860-7d5d-4e9f-9b43-08867f0ce8da)

### 4.2.Palancas 

Modelamiento de constantes de sistemas con palancas 

![image](https://github.com/user-attachments/assets/e6c4f00c-8d59-480f-a43f-f19b58e8b7a7)

### 4.3.Potenciómetro

En los potenciómetros hay dos tipos, por lo cual se generan dos tipos de modelamientos: los potenciómetros de rotación, en los que obtenemos:

![image](https://github.com/user-attachments/assets/8f095678-469f-4494-933a-ee5c9cc92659)

Y los de traslación, cuyo modelamiento de constantes es el siguiente:

![image](https://github.com/user-attachments/assets/bf195830-3552-4b9a-b0d4-0f7fe527ff71)

### 4.4.Tacómetros

* Son dispositivos que convierten la velocidad angular a voltaje, donde su modelaje se representa como:

![image](https://github.com/user-attachments/assets/3c1b9597-722d-4e75-8f58-1fa305c7272e)

![image](https://github.com/user-attachments/assets/96b84579-6233-45c0-9617-e2031c4ce664)

### 4.5.Sensores transmisores 

![image](https://github.com/user-attachments/assets/f4d2f55c-63e4-4cf0-a754-66269a083396)

En los sensores encontramos dos tipos de sensores, lo de medición lineal y los no lineales, cada uno tiene su propio modelado de ecuaciones. Los lienales se representan de la siguiente manera:

![image](https://github.com/user-attachments/assets/bc19c3b5-d758-4e89-9d7a-ae8cbc8f5a77)

* Los no lineales:

![image](https://github.com/user-attachments/assets/bbd09079-935b-4c18-bfbe-b74cbb934c36)

### 4.6.Modelos de otros procesos 

En este caso nos mostraron el análisis de la mezcla de sustancias en un tanque y por medio de un agitador

![image](https://github.com/user-attachments/assets/e83dc83f-b992-4b5b-a64c-4e6b1658ae5e)

Donde obtenemos que:  

![image](https://github.com/user-attachments/assets/c19d43d2-5af9-4465-b4e0-100825f9dbdb)

## 5.Conclusión

En esta clase se nos mostró el análisis y modelamiento por medio de un nuevo método el cual nos permite seccionar y analizar por separado para después juntar todas las ecuaciones o funciones de transferencia, además se nos dio una pequeña apertura a los diagramas de bloques y su representación.

## 6.Ejercicios extras 




