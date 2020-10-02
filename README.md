
# ROT13
import string
while True:
    abc = string.ascii_lowercase
    texto = str(input("Ingrese el texto a                         cifrar:"))
    if texto == '/':
        break
    else:
        for letra in texto.lower():
            if letra in abc:
                posicion = abc.index(letra) + 13
                if posicion > len(abc):
                    posicion1 = len(abc) -                                  (abc.index(letra) + 1)
                    posicion2 = 13 - (posicion1 +                                       1)
                    print(abc[posicion2], 
                          end = "") 
                elif (letra == 'n'):
                    print(abc[0], end = "")
                else:
                    print(abc[posicion], end =                             "")
            else:
                print(letra, end = "")
      print("")
