# Modelamiento Sistemas Mecanicos 
Se formula una ecuación a partir de un análisis matemático para sistemas mecánicos, teniendo como base ciertas representaciones de componentes mecánicos.
## 1Componentes
### 1.1.1Resorte 
$$F=kx=k(x_{1}-x_{2})$$

Donde k es la constante de elasticidad.

![Captura de pantalla 2025-04-30 095921](https://github.com/user-attachments/assets/0c3287ab-dbd0-4a04-8f0d-f5fb83d55d7c)

### 1.1.2Amortiguador 
$$F=b(x^{'})=k((x^{'}_{1})-(x _{2}^{'}))$$

Donde b es la constante de fricción viscosa.

![image](https://github.com/user-attachments/assets/06c8eb4a-a843-465e-9877-943e9f7213b6)

## 1.2Tipos de Friccion
Los dos tipos de fricción más usados son la fricción $$F_{R}$$ y la fricción viscosa  $$F_{F}$$

![image](https://github.com/user-attachments/assets/14cc5280-36ee-40cf-bf84-83ff98501c39)

### 1.2.1Friccion 

  $$F_{R}= K_{2} * y(t)$$ --> Ley de Hooke

### 1.2.2Friccion Viscosa

  $$F_{F}= K_{1} * y^{'}(t)$$ -->Friccion Viscosa

## 2.Ley de Newton 

 $$F= m*a$$

 ## 3.Sistemas Masa-Resorte-Amortiguador

Para empezar la modelación matemática de un sistema mecánico, se debe realizar un diagrama de cuerpo libre. Una vez elaborado, se procede a hacer un análisis mediante las leyes de Newton, teniendo en cuenta que la fuerza será el resultado de la suma y resta de las componentes que actúan sobre la masa.

En este análisis, u representa la entrada que recibirá el sistema;  $$F_{R}$$ se opone al movimiento y donde $$F_{F}$$ también se opondrá a la señal de entrada.

  💡**Ejemplo 1:**

  ![image](https://github.com/user-attachments/assets/dc5d19e9-c117-4349-a51e-6317d1da426a)

Se realiza un diagrama de cuerpo libre para cada una de las masas.

**Masa 1:**
![image](https://github.com/user-attachments/assets/dbf2c8f0-0468-4be7-bf1a-e4eec1e11343)

**Masa 2:**

![image](https://github.com/user-attachments/assets/aaf3c055-aeab-4fa3-90e3-46fabc8ffc01)

**Analisis m1:**

$$u-F_{F}-F _{R1}-F _{R2}-F _{F}=m _{1}*a _{m1}$$

$$u_ {t} -k _ {1}* x _ {1} (t)-k  _ {2} * (x _{1}(t)- x _{2}(t))-b* \frac{d(x _{1}(t)-x _{2}(t)}{dt}=m _{1}*\frac{d^{2}x _{1}(t)}{dt^{2}}$$
 
**Analisis m2:**

$$F _{R2}+F _{F}-F _{R3}=m _{2}*a _{m2}$$

$$k _{2}* (x _{1}(t)- x _{2}(t))+b* \frac{d(x _{1}(t)-x _{2}(t))}{dt}- k _{3}* x _{2}(t)=m _{2}*\frac{d^{2}x _{2}(t)}{dt^{2}}$$

## 4.Sistemas Rotacionales 

El análisis es muy parecido al del sistema mecánico, pero ahora, en lugar de un movimiento lineal, se trata de un movimiento rotacional.

### 4.1Adaptacion de bases matematicas 

 $$F_{R}= K_{2} * y(t)$$ --> $$F_{R}= K_{2} * \phi$$ --> $$\phi$$ es el angulo de torsion
 
 $$F_{F}= K_{1} * y^{'}(t)$$ --> $$F_{F}=b * \phi^{'}$$ --> $$\phi^{'}$$ es la velocidad angular

 $$F= m*a$$ --> $$T= J * \phi^{''}$$ --> J es el momento de inercia 

 ### 4.2Analisis de sitemas 

Muy parecido a los otros sistemas, primero se realiza un diagrama de cuerpo libre y se genera la ecuación representativa, teniendo en cuenta que $$T(t)$$ es la entrada del sistema, y que $$F_{R}$$ y $$F_{F}$$  se opone a la 
 entrada.

  💡**Ejemplo 2:**

  ![image](https://github.com/user-attachments/assets/05f424cb-f9c4-49af-b40f-fd95a6915128)

  **Diagrama de cuerpo libre:**

  ![image](https://github.com/user-attachments/assets/b5ed2526-764c-4e1c-9da1-f4181296cde7)

**Analisis de sistema:**

$$T _{t} -F _{F}-F _{R}=j *a$$ --> aceleracion angular

$$T {(t)} -k * \theta(t) -b *\frac{d\theta (t)}{dt}=J *\frac{d^{2}\theta(t) }{dt^{2}}$$

## 5.Conclusion 
En conclusión, en esta clase recibimos una breve introducción al análisis y modelamiento de sistemas dinámicos de tipo mecánico. También aprendimos a incorporar en las ecuaciones las características dinámicas de los componentes y sistemas.
