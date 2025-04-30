 # Correccion Parcial primer corte
En este documento se muestra y señala el proceso para conseguir las respuestas correctas del parcial del primer corte:
## 1. primer ejercicio
$$2x^{''}+2x^{'}+x=1$$
### Condiciones iniciales
$$x_{0}=0$$ 
$$x^{'}_{0}=2$$

$$2[s^{2}X_{(s)}-sx_{(0)}-x_{(0)}^{'}]+2[sX_{(s)}-x_{(0)}]+X_{s}=\frac{1}{s}$$
$$2s^{2}X_{(s)}-4+2sX_{(s)}+X_{s}=\frac{1}{s}$$
$$X_{(s)}(2s^{2}+2s+1)=\frac{1}{s}+4$$
$$X_{(s)}=\frac{4s+1}{s(s^{2}+2s+1)}=\frac{A}{s}+\frac{Bs+C}{(s^{2}+2s+1)}$$
$$A=1$$
$$B=-2$$
$$C=2$$
Despues de realizar un proceso algebraico y un complemento de cuadrado se puede obtener la inversa de laplace y obtenemos:
$$\frac{4s+1}{s(s^{2}+2s+1)}=\frac{1}{(s)}+\frac{-2s+2}{(s^{2}+2s+1)}=1+e^{-1/2t}(sin((1/2)t)-cos((1/2)t)$$
## 2. segundo ejercicio
$$F(s)=\frac{6s}{(s-(\frac{5}{2}))(s^{2}-4s+8)}$$
$$X_{(s)}=\frac{6s}{(s-(\frac{5}{2}))(s^{2}-4s+8)}=\frac{A}{(s-(\frac{5}{2}))}+\frac{Bs+C}{(s^{2}-4s+8)}$$
$$6s=A(s^{2}-4s+8)+(Bs+c)(s-(\frac{5}{2}))$$
$$A=\frac{60}{17}$$
$$B=-\frac{60}{17}$$
$$C=\frac{192}{17}$$
Despues de realizar un proceso algebraico y un complemento de cuadrado se puede obtener la inversa de laplace y obtenemos:
$$\frac{\frac{60}{17}}{(s-(\frac{5}{2}))}+\frac{-\frac{60}{17}s+\frac{192}{17}}{(s^{2}-4s+8)}=\frac{60}{17}e^{\frac{5}{2}t}+\frac{60}{17}cos(2t)e^{2t}+\frac{192}{17}e^{2t}sin(2t)$$
