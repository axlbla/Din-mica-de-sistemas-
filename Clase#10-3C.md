# Modelamiento de sitemas con diagramas de bloques 

Metodo para modelar sitemas complejos o compuestos de diferentes sub sistemas de manera mas sencilla por medio de funciones de transferencia,señales de entradas y salidas.Apoyandonos de un nuevo metodo llamado diagrama de bloques 

## 1.Sistemas conocidos 

Para  empezar el modelamiento de un sistema por medio de diagramas de bloques empezamos haciendo el analisis del sistemas , haciendo una particion del mismo con el siguiente ejemplo vamos mostrando como hacer el analisis en cada caso que se nos presenta.

💡**Ejemplo 1:** Vamos hacer el analisis de un soleniode por medio del modelamiento de diagrama de bloques

![image](https://github.com/user-attachments/assets/71628b30-3782-4749-9208-864e3e6f1a4e)


### 1.1Sistemas electricos

Metodo para el analisis de sistemas electricos:

💡**Ejemplo 1:** Se realiza el analisis de un solenoide haciendo primero en analisis electrico del sistema.

![WhatsApp Image 2025-06-12 at 9 40 47 AM](https://github.com/user-attachments/assets/ffc4dfe7-dd0b-4e4a-9bcf-a3177dd17156)

Primero hacemos un analisis electrico utilizando el metodo de mallas donde obtenemos:

$$L\frac{\mathrm{d}i }{\mathrm{d} t}+Ri=V _{(t)}$$

Aplicando la place y despejando la funcion de transferencia tenemos 

$$\frac{I _{(s)}}{ V _{(S)}} = \frac{1}{Ls+R}$$

### 1.2Sistemas de transformacion de energia

Son sistemas que se encarga de transformar una energia entrante en otro tipo de energia ya sea mecanica, electrica o rotacional. Normalmente se representan con constantes o relaciones proporcionadas.

💡**Ejemplo 1:** Siguendo con el ejemplo anterior tenemos el analisis del sistema transductor 

* Relacion electrica con la mecanica donde tenemos que:

  $$f _{(s)} = k _{s} * i$$

Donde tenemos que $$k _{s}$$ es una constante.Aplicando laplace y obteniendo la funcion de transferencia se obtiene que:

$$\frac{F _{(s)} }{I _{(s)}} = K _{s}$$

### 1.3Sistemas Mecanicos 

Metodo para el analisis de sistemas mecanicos, muy parecido al analisis mecanico se plantean las ecuaciones pero ahora se generan funciones de transferencia.

💡**Ejemplo 1:** Siguendo con el ejemplo anterior hacemos el analisis mecanico de los solenoides 

![WhatsApp Image 2025-06-12 at 9 41 02 AM](https://github.com/user-attachments/assets/44391c5f-444e-4df4-836a-6a654a060473)

Haciendo el analisis mecanico obtenemos la siguiente ecuacion diferencial:

$$f _{(t)} - kx-bx^{'}= mx^{''}$$

Aplicando laplace y dejando en terminos de la funcion de transferencia obtenemos que:

$$\frac{X _{(s)}}{F _{(s)}} = \frac{1}{ms ^{2}+ bs + k}$$

##  2.Represnetacion de bloques 

Para representar un sistema en diagramas de bloques solo se deben tener n cuenta dos cosas. la primera es la funcion de transferencia la segunda son las señales de entradas y salidas 

💡**Ejemplo 1:** Siguendo con el ejemplo anterior hacemos la representacion de diagrama de bloques del solenoides 

![image](https://github.com/user-attachments/assets/98524473-8481-4955-906b-9f20fcfd464d)

Como podemos apreciar la representacion nos indica que variable nos va ha entregar de cada uno de los subsistemas  como tambien la variable de salida que nos entrega el sistema, en este caso, un movimiento lineal cuando nos dan un voltaje.

## 3.Modelamiento de Sistemas mas comunes 

En esta parte de la clase nos enseñaron el modelamineto de un motor DC de dos formas, utilizando el mismo metodo de modelamiento de diagramas de bloques.

![image](https://github.com/user-attachments/assets/9b5ce080-2660-44d3-9cb0-1b8931b1114b)

los dos metodos para analisar un Motor Dc son:

* Corriente de campo
* Corriente de armadura

En estos apunte veremos un resumen de cada metodo y sus resultados.

### 3.1Corriente de Campo

#### 3.1.1Analisis electrico del motor 

Para este analisis se hace mallas pero se hace la suposicion que la corriente de armadura es constante.

![image](https://github.com/user-attachments/assets/fe398716-ce0e-4ccd-a950-377f012f4cd1)

Despues de hacer el analisis obtenemos que:

$$\frac{I _{(s)}}{ V _{(S)}} = \frac{1}{L _{(c)}s+R _{(c)}}$$


#### 3.1.2Analisis Electromecanico(sub-Sistema de transformacion de energia)

Para este analisis se deben tener en cuentas varias constantes y igualdades de transformacion.Tales como 

* El flujo en el entrehierro es proporcional a la corriente de campo
  
$$\phi = k _{c} i _{c}$$

* El torque desarrollado es porporcional al flujo y a la corriente de armadura.En esta realcion todas las constantes $$(k _{c} i _{c} k _{a})$$ se vuelven $$K _{m}$$ asi obtenemos.

$$T _{m}= (k _{m}) I _{c (s)}$$
  
* El torque aplicado a la carag es el realizado por el motor menos la inercia de la carga

$$T _{c(s)}= T _{m(s)} - T _{p(s)}$$

![image](https://github.com/user-attachments/assets/b4e3324d-612f-4dbc-82d1-249b03c7ab5b)

#### 3.1.3Analisis mecanico de la carga y el torque 

En este sistema se realiza un analisis mecanico teniendo en cuenta la carga los momentos de inercia y el torque del motor 

![image](https://github.com/user-attachments/assets/c3f6d285-72e1-46a4-a3b5-d3f13909ba0b)

* Obtenemos la ecuacion mecanica

$$J \frac{d^2 \theta  }{d t^2} + b\frac{\mathrm{d} \theta  }{\mathrm{d} t} + k\theta  = \tau _{(t)}$$

Haciendo la funcion de transferencia obtenemos que:

$$\frac{\theta _{s}}{T _{c(s)}} = \frac{1}{(js ^{2} + bs)}$$

#### 3.1.4Representacion de Diagramas de bloques 

Como penultimo paso vamos a remplazar en las ecuaciones obtenidas en el sistema de transformacion para asi empezar el analisis de los diagramas de bloques obteniendo:

$$\theta _{s} = \frac{K _{m}}{(L _{(c)}s +R _{(c)})(js ^{2} + bs)} - T _{p(s)}\frac{1}{(js ^{2} + bs)}$$

Ya por ultimo hacemos la representacion de diagramas de bloques obteniendo 

![image](https://github.com/user-attachments/assets/4923b3b7-6e8c-4129-ab30-9d472321fde1)

### 3.1Corriente de Armadura

#### 3.2.1Analisis electrico del motor 

Para este analisis se hace mallas pero se hace la suposicion que la corriente de campo es constante.

![image](https://github.com/user-attachments/assets/1567eea7-8ba4-4477-bca2-0ae54717ec20)

Despues de hacer el analisis obtenemos que:

$$\frac{I _{(s)}}{ V _{(S)}} = \frac{1}{L _{(a)}s+R _{(a)}}$$


#### 3.2.2Analisis Electromecanico(sub-Sistema de transformacion de energia)

Para este analisis se deben tener en cuentas varias constantes y igualdades de transformacion.Tales como:

* La corriente de armadura se relaciona con el voltaje  aplicado a la armadura.En este analisis se realcionan todas las constantes $$(k _{c} i _{c} k _{a})$$ haciendo que se vuelvan $$K _{m}$$ asi obtenemos:

$$T _{m}= (k _{m}) I _{a (s)}$$

* Se realiza una relacion entre los voltajes y los torques, obteniendo:

$$V _{a(s)}= L _{(a)}s+R _{(a)}I _{a (s)} + V _{b(s)}$$

* El voltaje inducido en la armadura es porporcional a la velocidad angular del eje:

$$V _{b(s)}= k _{b} w _{s}$$

* Al remplazar en las ecuaciones se obtiene

$$I _{(s)}= \frac{V _{a(s)}-k _{b} w _{s}}{ L _{(a)}s + R _{(a)}}$$

![image](https://github.com/user-attachments/assets/899ab540-e4ee-45e2-bd7e-db63988d29f1)

#### 3.2.3Analisis mecanico de la carga y el torque 

* El torque aplicado a la carag es el realizado por el motor menos la inercia de la carga

  $$T _{c(s)}= T _{m(s)} - T _{p(s)}$$

* En este sistema se realiza el mismo analisis mecanico que en metodo anterior, teniendo en cuenta la carga ,los momentos de inercia y el torque del motor 

$$\frac{\theta _{s}}{T _{c(s)}} = \frac{1}{(js ^{2} + bs)}$$

![image](https://github.com/user-attachments/assets/ddab7660-6470-4531-ac13-77e65646f2b4)


#### 3.1.4Representacion de Diagramas de bloques 

Ya por ultimo hacemos la representacion de diagramas de bloques obteniendo.

![image](https://github.com/user-attachments/assets/bfcbe3f9-40b8-4f4d-9fbd-7e5bfbfedc3a)

## 4.Relaciones de componentes en sistemas 

Son relaciones de constantes dinamicas para hacer la transformacion de energia en los sistemas  dinamicos de estas hay mecanicas , electricas , hidrualicas, etc.

### 4.1Engranajes y Poleas 

Son dispositivos mecanicos que trasmiten la energia desde una parte del sistema a otra

