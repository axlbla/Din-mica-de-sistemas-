# Terminación de Tema y MATLAB

## 1.Descomposición en Fracciones Parciales 

 ### 1.1Caso 2

En este caso, analizamos la situación en la que las raíces son iguales. Se tiene una transformada, y al aplicar su inversa, se descompone en fracciones parciales con raíces repetidas.

 💡 **Ejemplo 1:** Obtenga la transformada inversa de:

  $$G(s)=\frac{2s^{2}+6s+5}{(s+2)(s+1)^{2}}$$

  $$\frac{2s^{2}+6s+5}{(s+2)(s+1)^{2}}=\frac{A}{(s+2)}+\frac{B}{(s+1)}+\frac{c}{(s+1)^{2}}$$

  $$2s^{2}+6s+5=A(s+1)^{2}+B(s+2)(s+1)+C(s+2)$$

  $$A=1$$

  $$B=1$$

  $$C=1$$
 
$$g(t)=e^{-2t}+e^{-t}+te^{-t}$$

# 1.1.1 Ejercicios

📚
a)Encuentre f(t):

$$F(s)=\frac{s^{2}+2s+3}{(s+1)^{3}}$$

$$\frac{s^{2}+2s+3}{(s+1)^{3}}=\frac{A}{(s+1)}+\frac{B}{(s+1)^{2}}+\frac{C}{(s+1)^{3}}$$

  $$s^{2}+2s+3=A(s+1)^{3}+B(s+1)^{2}+C$$

$$A=1$$

$$B=0$$

$$C=2$$

$$f(t)=e^{-t}+t^{2}e^{-t}$$

b)📚

$$F(s)=\frac{2s^{2}+1}{(s-2)^{3}}$$

$$\frac{2s^{2}+1}{(s-2)^{3}}=\frac{A}{(s-2)}+\frac{B}{(s-2)^{2}}+\frac{C}{(s-2)^{3}}$$

$$2s^{2}+1=A(s-2)^{3}+B(s-2)^{2}+C$$

$$A=2$$

$$B=8$$

$$C=9$$

$$f(t)=2e^{t}+8te^{2t}+\frac{9t^{2}e^{2t}}{2}$$

 ### 1.2Caso 3

En este caso, analizamos el método de solución cuando las fracciones parciales se descomponen con raíces complejas y conjugadas.

💡 **Ejemplo 1:** Obtenga la transformada inversa de:

$$G(s)=\frac{s^{2}+2s+3}{(s^{2}+2s+2)(s^{2}+2s+5)}$$

$$\frac{s^{2}+2s+3}{(s^{2}+2s+2)(s^{2}+2s+5)}=\frac{As+B}{(s^{2}+2s+2)}+\frac{Cs+D}{(s^{2}+2s+5)}$$

$$s^{2}+2s+3=(As+B)(s^{2}+2s+5)+(Cs+D)(s^{2}+2s+2)$$

$$A=0$$

$$B=\frac{1}{3}$$

$$C=0$$

$$D=\frac{2}{3}$$

Se completa el cuadrado 

$$\frac{\frac{1}{3}}{s^{2}+2s+2+1-1}+\frac{\frac{2}{3}}{s^{2}+2s+5-4+4}$$

$$\frac{\frac{1}{3}}{(s+1)^{2}+1}+\frac{\frac{2}{3}}{(s+1)^{2}+4}$$

$$g(t)=\frac{1}{3}e^{-t}sen(t)+\frac{1}{3}e^{-t}sen(2t)$$

# 1.2.1 Ejercicios

📚
a)Encuentre f(t):

$$F(s)=\frac{3s+5}{9s^{2}-12s+20}$$

$$\frac{3s+5}{9s^{2}-12s+20}=\frac{As+B}{9s^{2}-12s+20}$$

$$3s+5=As+B$$

$$A=3$$

$$B=5$$

$$\frac{3s+5}{9s^{2}-12s+20}$$

Se completa el cuadrado

$$9(s^{2}-12s+20)=9(s^{2}-\frac{12s}{9}+\frac{20}{9})=9(s^{2}-\frac{4s}{3}+\frac{20}{9})=9[(s^{2}+\frac{4s}{3}+(\frac{2}{3})^{2})+\frac{20}{9}-(\frac{2}{3})^{2}]$$

$$9[(s-\frac{2}{3})^{2}+\frac{16}{9}]$$

$$\frac{3s+5}{9[(s-\frac{2}{3})^{2}+\frac{16}{9}]}$$

$$\frac{3s+5}{9[(s-\frac{2}{3})^{2}+\frac{16}{9}]}=\frac{1}{9}[\frac{3(s-\frac{2}{3}+\frac{2}{3})5}{[(s-\frac{2}{3})^{2}+\frac{16}{9}]}]=\frac{1}{9}[\frac{3(s-\frac{2}{3})+3(\frac{2}{3})+5}{[(s-\frac{2}{3})^{2}+\frac{16}{9}]}]=\frac{1}{9}[\frac{3(s-\frac{2}{3})}{[(s-\frac{2}{3})^{2}+\frac{16}{9}]}+\frac{7}{(s-\frac{2}{3})^{2}+\frac{16}{9}}]$$

$$\frac{1}{9}[\frac{3(s-\frac{2}{3})}{[(s-\frac{2}{3})^{2}+\frac{16}{9}]}+\frac{7}{(s-\frac{2}{3})^{2}+\frac{16}{9}}]=(\frac{3}{9})\frac{(s-\frac{2}{3})}{(s-\frac{2}{3})^{2}+\frac{16}{9}}+(\frac{7}{9})\frac{1}{(s-\frac{2}{3})^{2}+\frac{16}{9}}$$

$$(\frac{3}{9})\frac{(s-\frac{2}{3})}{(s-\frac{2}{3})^{2}+\frac{16}{9}}+(\frac{7}{9})\frac{1}{(s-\frac{2}{3})^{2}+\frac{16}{9}}=(\frac{3}{9})\frac{(s-\frac{2}{3})}{(s-\frac{2}{3})^{2}+\frac{16}{9}}+(\frac{7}{9})*\frac{3}{4}\frac{\frac{4}{3}}{(s-\frac{2}{3})^{2}+\frac{16}{9}}$$

$$f(t)=(\frac{3}{9})\frac{(s-\frac{2}{3})}{(s-\frac{2}{3})^{2}+\frac{16}{9}}+(\frac{7}{9})*\frac{3}{4}\frac{\frac{4}{3}}{(s-\frac{2}{3})^{2}+\frac{16}{9}}=\frac{1}{2}e^{\frac{2}{3}t}cos(\frac{4}{3}t)+\frac{7}{12}e^{\frac{2}{3}t}sen(\frac{4}{3}t)$$

📚
b)Encuentre f(t):


$$F(s)=\frac{2}{s(s^{2}+1)}$$

$$\frac{2}{s(s^{2}+1)}=\frac{A}{s}+\frac{Bs+C}{s^{2}+1}$$

$$2=A(s^{2}+1)+(Bs+C)(s)$$

$$C=0$$

$$A=2$$

$$B=-2$$

$$f(t)=2-cos(t)$$


## 2.Matlab 

En esta clase se nos dio una breve descripción de cómo solucionar transformadas, fracciones parciales y transformadas inversas en MATLAB. Utilizamos como ejemplos los ya resueltos en clase para comparar.

💡 **Ejemplo 1:** Obtenga la transformada inversa en matlab de:

$$G(s)=\frac{2s^{2}+6s+5}{(s+2)(s+1)^{2}}$$

```
  syms s t
y=(2*s^{2}+6*s+5)/((s+2)*(s+1)^{2})
y= ilaplace(y)
 
y =
 
(2*s^2 + 6*s + 5)/((s + 1)^2*(s + 2))
 
 
y =
 
exp(-t) + exp(-2*t) + t*exp(-t)
 ```

💡 **Ejemplo 2:** Obtenga la transformada inversa en matlab de:



$$G(s)=\frac{s^{2}+2s+3}{(s^{2}+2s+2)(s^{2}+2s+5)}$$

```
 syms s t
y=(s^{2}+2*s+3)/((s^{2}+2*s+2)*(s^{2}+2*s+5))
y=ilaplace(y)
 
y =
 
(s^2 + 2*s + 3)/((s^2 + 2*s + 2)*(s^2 + 2*s + 5))
 
 
y =
 
(exp(-t)*sin(t))/3 + (sin(2*t)*exp(-t))/3
 
```
# 2.1 ejercicios 

📚
a)Encuentre f(t):


$$F(s)=\frac{s^{2}+2s+3}{(s+1)^{3}}$$

```
 syms s t
y=(s^{2}+2*s+3)/(s+1)^{3}
y=ilaplace(y)
 
y =
 
(s^2 + 2*s + 3)/(s + 1)^3
 
 
y =
 
exp(-t) + t^2*exp(-t)
```

📚
b)Encuentre f(t):


$$F(s)=\frac{3s+5}{9s^{2}-12s+20}$$

```
 syms s t
y=(3*s+5)/(9*s^{2}+12*s+20)
y=ilaplace(y)
 
y =
 
(3*s + 5)/(9*s^2 + 12*s + 20)
 
 
y =
 
(exp(-(2*t)/3)*(cos((4*t)/3) + (3*sin((4*t)/3))/4))/3

```

## 3.Conclusión 
Aprendimos los últimos casos de fracciones parciales. También aprendimos a utilizar la herramienta de MATLAB para resolver y comparar tanto transformadas como sus inversas.

## 4.Referencias 
Punto a caso 3:
* https://www.youtube.com/watch?v=6Yfd2oZMQ4M

Punto b caso 3:
* https://www.youtube.com/watch?v=Eqr_zKdDfZI

Punto b caso 2:
* https://www.youtube.com/watch?v=HZZ9SFTFlyo

Punto a caso 2:
* https://www.youtube.com/watch?v=FbgiLLyrpso
