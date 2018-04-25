import math
from math import sqrt
print("Primeira tela:\nparte do código sobre a visão da álgebra da equação da parábola")
print('\n'*2)
a = int(input("Digite o A:"))
b = int(input("Digite o B:"))
c = int(input("Digite o C:"))
delta = b**2-4*a*c
X1 = (-b-math.sqrt(delta))/2*a
X2 = (-b+math.sqrt(delta))/2*a
Xv = -b/2*a
Yv = -delta/4*a
if type(a) == int:
    if delta > 0:
        print("O vértice da parábola está no ponto V({}, {})".format(Xv, Yv))
        print("Suas raízes são X1 = {} e X2 = {} e seu Delta = {}".format(X1, X2, delta))
    elif delta == 0:
        print("O vértice da parábola está no ponto V({}, {})".format(Xv, Yv))
        print("Suas raízes são iguais e valem {} e seu Delta = {}".format(X1, delta))
    else:
        print("O vértice da parábola está no ponto V({}, {})".format(Xv, Yv))
        print("Suas raízes não são Reais, mas seu Delta =", delta)
print('='*40)
print("Segunda tela:\nparte do código sobre a visão da geometria analítica da parábola")
print('\n'*2)
print('Construção da equação da reta a partir de 2 pontos distintos, A e B, no plano')
print('Defina as coordenadas X e Y dos pontos, respectivamente')
    #Definindo o valor dos pontos
Ax = int(input('Ax = '))
Ay = int(input('Ay = '))
Bx = int(input('Bx = '))
By = int(input('By = '))
x = Bx - Ax
y = By - Ay
m = int(y/x)
distancia = sqrt(x**2 + y**2)

    #Definindo a nossa função do 1º grau: y = yo + m(x - xo)
if m > 0:
    print('Sua função é: y = {0}*x + {1}'.format(Ax, Ax+m*Ay))
    print('A função é crescente, pois: m (taxa de variação) > 0')
elif m < 0:
    print('Sua função é: y = {0}*x + {1}'.format(Ax, Ax + m * Ay))
    '''Ax+m*Ay'''
    print('A função é decrescente, pois: m (taxa de variação) < 0')
else:
    print('Sua função é: y = {0}*x + {1}'.format(Ax, Ax + m * Ay))
    print('Reta constante, m = 0')
    # Distância entre os pontos A e B
    print('A distância entre o ponto A e B é de {:.4f} unidades de medida.'.format(distancia))
