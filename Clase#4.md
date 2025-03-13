# Método Resumido 
Se nos explica un segundo método para solucionar los tres casos de fracciones parciales 

## 1.Fracciones Parciales Metodo Resumido 
En este método, aprovechamos la multiplicación de las componentes del denominador con las componentes del numerador en todas las fracciones parciales. Esto permite que muchas de las componentes se simplifiquen, facilitando así la búsqueda de las incógnitas. 

### 1.1.Caso 1: Raices Reales y Diferentes
En este caso, buscaremos solucionar las fracciones parciales cuando las raíces son reales y diferentes, utilizando un nuevo método.

💡**Ejemplo 1:** Encontrar f(x):

$$F(s)=\frac{s+3}{(s+1)(s+2)}$$

$$\frac{s+3}{(s+1)(s+2)}=\frac{A}{(s+1)}+\frac{B}{(s+2)}$$

$$[\frac{(s+1)(s+3)}{(s+1)(s+2)}] _{(s=-1)}= [\frac{(s+1)A}{(s+1)}+\frac{(s+1)B}{(s+2)}] _{(s=-1)}$$


$$A=2$$

$$[\frac{(s+2)s+3}{(s+1)(s+2)}]_{(s=-2)}=[\frac{(s+2)A}{(s+1)}+\frac{(s+2)B}{(s+2)}] _{(s=-2)}$$

$$B=-1$$

$$f(x)=\frac{2}{(s+1)}+\frac{-1}{(s+2)}=2e^{-t}-e^{-2t}$$

# 1.1.1 Ejercicios 

📚
a)Encuentre f(t):

$$F(s)=\frac{2s+7}{(s-9)(s+5)}$$

$$\frac{(2s+7)}{(s-9)(s+5)}=\frac{A}{(s-9)}+\frac{B}{(s+5)}$$

$$[\frac{(s-9)(2s+7)}{(s-9)(s+5)}] _{(s=9)}= [\frac{(s-9)A}{(s-9)}+\frac{(s-9)B}{(s+5)}] _{(s=9)}$$

$$A=\frac{25}{14}$$

$$[\frac{(s+5)(2s+7)}{(s-9)(s+5)}] _{(s=-5)}= [\frac{(s+5)A}{(s-9)}+\frac{(s+5)B}{(s+5)}] _{(s=-5)}$$

$$B=\frac{3}{14}$$

$$f(t)=\frac{25}{14}e^{9t}+\frac{3}{14}e^{-5t}$$

📚
b)Encuentre f(t):

$$F(s)=\frac{s-1}{(s-2)(s-3)}$$

$$\frac{(s-1)}{(s-2)(s-3)}=\frac{A}{(s-2)}+\frac{B}{(s-3)}$$

$$[\frac{(s-2)(s-1)}{(s-2)(s-3)}] _{(s=2)}= [\frac{(s-2)A}{(s-2)}+\frac{(s-2)B}{(s-3)}] _{(s=2)}$$

$$A=-1$$

$$[\frac{(s-3)(s-1)}{(s-2)(s-3)}] _{(s=3)}= [\frac{(s-3)A}{(s-2)}+\frac{(s-3)B}{(s-3)}] _{(s=3)}$$

$$B=2$$

$$f(t)=-e^{2t}+2e^{3t}$$

### 1.2.Caso 2: Raices Reales y iguales

En este caso, buscaremos solucionar las fracciones parciales cuando las raíces son reales e iguales, utilizando un nuevo método

💡**Ejemplo 1:** Encontrar f(x):

$$F(s)=\frac{s^{2}+2s+3}{(s+1)^{3}}$$

$$\frac{s^{2}+2s+3}{(s+1)^{3}}=\frac{A}{(s+1)}+\frac{B}{(s+1)^{2}}+\frac{C}{(s+1)^{3}}$$

$$\frac{(s^{2}+2s+3)(s+1)^{3}}{(s+1)^{3}}=A+B(s+1)+C(s+1)^{2}$$

$$[\frac{(s^{2}+2s+3)(s+1)^{3}}{(s+1)^{3}}] _{s=-1}=[A+B(s+1)+C(s+1)^{2}] _{s=-1}$$

$$C=2$$

$$\frac{d}{ds}[s^{2}+2s+3] _{(s=-1)}=[A+B(s+1)+C(s+1)^{2}] _{(s=-1)}$$

$$\frac{d}{ds}[2s+2] _{(s=-1)}=[B+2C(s+1)] _{(s=-1)}$$

$$B=0$$

$$\frac{d^{2}}{ds^{2}}[2] _{(s=-1)}=[2C] _{(s=-1)}$$

$$A=1$$

$$\frac{s^{2}+2s+3}{(s+1)^{3}}=\frac{1}{(s+1)}+\frac{0}{(s+1)^{2}}+\frac{2}{(s+1)^{3}}$$

$$f(t)=(t^{2}+1)e^{-t}$$

# 1.2.1 Ejercicios 

📚
a)Encuentre f(t):

$$F(s)=\frac{2s^{2}+1}{(s-2)^{3}}$$

$$\frac{2s^{2}+1}{(s-2)^{3}}=\frac{A}{(s-2)}+\frac{B}{(s-2)^{2}}+\frac{C}{(s-2)^{3}}$$

$$[2s^{2}+1] _{(s=2)}=[A(s-2)^{2}+B(s-2)+C] _{(s=2)}$$

$$C=9$$

$$\frac{d}{ds}[4s] _{(s=2)}=[2A(s-2)+B] _{(s=2)}$$

$$B=8$$

$$\frac{d^{2}}{ds^{2}}[4] _{(s=2)}=[2A] _{(s=2)}$$

$$A=2$$

$$\frac{2s^{2}+1}{(s-2)^{3}}=\frac{2}{(s-2)}+\frac{8}{(s-2)^{2}}+\frac{9}{(s-2)^{3}}$$

$$f(t)=2e^{t}+8te^{2t}+\frac{9t^{2}e^{2t}}{2}$$

📚
b)Encuentre f(t):

$$F(s)=\frac{2s^{2}+6s+5}{(s+1)^{2}}$$

$$\frac{2s^{2}+6s+5}{(s+1)^{2}}=\frac{A}{(s+1)}+\frac{B}{(s+1)^{2}}$$

$$[2s^{2}+6s+5] _{(S=-1)}=[A(s+1)+B] _{(S=-1)}$$

$$B=1$$

$$\frac{d}{ds}[4s+6] _{(S=-1)}=[A]_{(S=-1)}$$

$$A=2$$

$$f(x)=2e^{-t}+e^{-t}t$$

### 1.3.Caso 3: Raices complejas y conjugadas 

En este caso, veremos cómo solucionar fracciones parciales con raíces complejas y conjugadas utilizando el método resumido.

💡**Ejemplo 1:** Encontrar f(x):

$$F(s)=\frac{2s+12}{s^{2}+2s+5}$$

Se completa el cuadrado 

$$\frac{2(s+6)}{(s+1)^{2}+4}=2[\frac{(s+6)}{(s+1)^{2}+4}]=2[\frac{(s+1)-1+6}{(s+1)^{2}+4}]=[2\frac{(s+1)}{(s+1)^{2}+4}+5\frac{2}{(s+1)^{2}+4}]$$

$$f(t)=5e^{-t}sen(2t)+2e^{-t}cos(2t)$$

# 1.3.1 Ejercicios 

📚
a)Encuentre f(t):

$$F(s)=\frac{3s+5}{9s^{2}-12s+20}$$

$$\frac{3s+5}{9s^{2}-12s+20}=\frac{As+B}{9s^{2}-12s+20}$$

se completa el cuadrado:

$$(\frac{3}{9})\frac{(s-\frac{2}{3})}{(s-\frac{2}{3})^{2}+\frac{16}{9}}+(\frac{7}{9})\frac{1}{(s-\frac{2}{3})^{2}+\frac{16}{9}}=(\frac{3}{9})\frac{(s-\frac{2}{3})}{(s-\frac{2}{3})^{2}+\frac{16}{9}}+(\frac{7}{9})*\frac{3}{4}\frac{\frac{4}{3}}{(s-\frac{2}{3})^{2}+\frac{16}{9}}$$


$$f(t)=\frac{1}{2}e^{\frac{2}{3}t}cos(\frac{4}{3}t)+\frac{7}{12}e^{\frac{2}{3}t}sen(\frac{4}{3}t)$$


📚
b)Encuentre f(t):

$$F(s)=\frac{2}{s(s^{2}+1)}$$

$$[\frac{s2}{s(s^{2}+1)}] _{(s=0)}= [\frac{As}{s}+\frac{s(Bs+C)}{s^{2}+1}] _{(s=0)}$$

$$A=2$$

$$[\frac{(s^{2}+1)2}{s(s^{2}+1)}] _{(s=i)}= [\frac{A(s^{2}+1)}{s}+\frac{(s^{2}+1)(Bs+C)}{(s^{2}+1)}] _{(s=i)}$$

$$C=0$$

$$B=-2$$

$$f(t)=2-cos(t)$$

## 2.Metodologia De solucion De Ecuaciones

En esta parte se realizó un mapeo general de los pasos a seguir para solucionar una ecuación. Primero, se aplica la transformada de Laplace, luego se descompone en fracciones parciales y, por último, se aplica la transformada inversa de Laplace para obtener sus componentes.

 
💡**Ejemplo 1:** Encontrar f(x):

$$x^{''}+2x^{'}+5x=3$$

$$x_{0}=0$$ 

$$x _{0}^{'}=0$$

$$[s^{2}X_{(s)}-sx_{(0)}-x_{(0)}^{'}]+2[sX_{(s)}-x_{(0)}]+5X_{s}=\frac{3}{s}$$

$$X_{(s)}=\frac{3}{s(s^{2}+2s+5)}=\frac{A}{s}+\frac{Bs+C}{(s^{2}+2s+5)}$$

$$A=\frac{3}{5}$$

$$B=\frac{-3}{5}$$

$$C=\frac{-6}{5}$$

$$f_{(x)}=\frac{3}{5}-\frac{3}{5}e^{-t}cos(2t)-\frac{3}{10}e^{-t}sen(2t)$$


## 3.Conlusion 

En esta clase aprendimos otro método para resolver fracciones parciales. También resolvimos ecuaciones mediante la transformada e inversa de Laplace. Además, tuvimos una breve explicación sobre el simulador Simulink y MATLAB.

## 4.Referencias 

*  https://www.youtube.com/watch?v=6Yfd2oZMQ4M

* https://www.youtube.com/watch?v=Eqr_zKdDfZI

* https://www.youtube.com/watch?v=HZZ9SFTFlyo

* https://www.youtube.com/watch?v=FbgiLLyrpso

* https://www.youtube.com/watch?v=HZZ9SFTFlyo

* https://www.youtube.com/watch?v=C3nEBf_Vgzg



