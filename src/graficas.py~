#! /usr/bin/python
import modulo
import matplotlib.pyplot as pl
x=[0.1,0.3,0.5,0.7,0.9]
def error (n,m,umbral):
    s=0
    for i in range(m):   
      apr1 = modulo.aproximacion(n)
      apr2 =modulo.aproximacion(n)
      if abs(modulo.aproximacion(n))-(modulo.aproximacion(n))> umbral:
        s+=1
    porcentaje=float((float(s)/float(n))*100)
    return porcentaje 
    
if __name__ =='__main__':
    n=int(raw_input('introduzca n'))
    m=int(raw_input('introduzca m'))
    y=[]
    for i in x:
      r = error(n,m,x)
      print 'El porcentaje de fallos es %f' % (r)
      y=y + [r]
pl.plot(x,y,'go')
pl.title('Dibujando umbral frente a porcentajes')
pl.xlim(-1.0,2.0)
pl.ylim(-2.0,2.0)
pl.show()