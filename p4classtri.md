# Prog.uff.25-1
Exercícios John Reed


#5 P4triang.py

#FUPPEEBQ

#1_ Leia os 3 lados reais de um triangulo;

#2_ Classifique: equilatero; isosceles; escaleno



#Inicio do codigo
print('Olá usuário! Bem vindo ao classificador de triângulos!')
print('Vamos começar?')
print('Insira valor do lado A:')
lA=(int(input()))
print('Insira valor do lado B:')
lB=(int(input()))
print('Insira valor do lado C:')
lC=(int(input()))
P=(lA + lB + lC) #perimetro
H=(P - lA)*(P - lB)*(P - lC)
if(H > 0):
    if(lA == lB):
      if(lB == lC):
        print('Esse triângulo é equilátero')
    else:
        if(lA == lB):
          if (lB != lC):
            print('Esse triângulo é isósceles')
        else:
            if(lA == lC):
              if(lB != lA):
                print('Esse triângulo é isósceles')
            else:
                if(lB == lC):
                  if(lC != lA):
                    print('Esse triângulo é isósceles')
                else:
                    print('Esse triângulo é escaleno')
else:
  print('Não é um triângulo')
#Fim do codigo
