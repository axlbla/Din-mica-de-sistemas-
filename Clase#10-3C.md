# Modelamiento de sitemas con diagramas de bloques 

Metodo para modelar sitemas complejos o compuestos de diferentes sub sistemas de manera mas sencilla por medio de funciones de transferencia,señales de entradas y salidas.Apoyandonos de un nuevo metodo llamado diagrama de bloques 

## Sistemas conocidos 

### Sistemas electricos

Metodo para el analisis de sistemas electricos:

💡**Ejemplo 1:** Se realiza el analisis de un solenoide haciendo primero en analisis electrico del sistema.

![WhatsApp Image 2025-06-12 at 9 40 47 AM](https://github.com/user-attachments/assets/ffc4dfe7-dd0b-4e4a-9bcf-a3177dd17156)

Primero hacemos un analisis electrico utilizando el metodo de mallas donde obtenemos:

$$L\frac{\mathrm{d}i }{\mathrm{d} t}+Ri=V _{(t)}$$

Aplicando la place y despejando la funcion de transferencia tenemos 

$$\frac{I _{(s)}}{ V _{(S)}} = \frac{1}{Ls+R}$$

### Sistemas de transformacion de energia

Son sistemas que se encarga de transformar una energia entrante en otro tipo de energia ya sea mecanica, electrica o rotacional. Normalmente se representan con constantes o relaciones proporcionadas.

💡**Ejemplo 1:** Siguendo con el ejemplo anterior tenemos el analisis del sistema transductor 

* Relacion electrica con la mecanica donde tenemos que:

  $$f _{(s)} = k _{s} * i$$

Donde tenemos que $$k _{s}$$ es una constante.Aplicando laplace y obteniendo la funcion de transferencia se obtiene que:

$$\frac{F _{(s)} }{I _{(s)}} = K _{s}$$


   
