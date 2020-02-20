# Programas-Teste
Códigos e Programas de teste e aprendizado
from random import*
#def onecoup(n):
    #p ='Duque,Capitao,Assassino,Condesa,Embaixador'.split(",")
    #for x in n:

def onecoup(n):
    influencia = ['Duque','Capitão','Assassino','Condessa','Embaixador']
    p = []
    if 8 <= len(n) <= 10:
        for x in influencia:
           for i in range(5):
               p.append(x)
        lista = []
        for x in n:
            i = choice(p)
            del p[p.index(i)]
            j = choice(p)
            del p[p.index(j)]
            lista.append(x + " é " + i + " e " + j)
        return lista,p
     
  elif 6 <= len(n) <= 7:
      for x in influencia:
      for i in range(5):
            p.append(x)
       lista = []
       for x in n:
           i = choice(p)
           del p[p.index(i)]
           j = choice(p)
           del p[p.index(j)]
           lista.append(x + " é " + i + " e " + j)
        return lista,p

    elif 3 <= len(n) <= 5:
       for x in influencia:
           for i in range(5):
               p.append(x)
       lista = []
       for x in n:
           i = choice(p)
           del p[p.index(i)]
           j = choice(p)
           del p[p.index(j)]
           lista.append(x + " é " + i + " e " + j)
        return lista, p

    elif len(n) == 2:
       for x in influencia:
           for i in range(5):
               p.append(x)
       lista = []
       for x in n:
           i = choice(p)
           del p[p.index(i)]
           j = choice(p)
           del p[p.index(j)]
           lista.append(x + " é " + i + " e " + j)
        return lista, p

    else:
       pass

print(onecoup("Júlio,Kayann,Henrique,Gabi".split(",")))
