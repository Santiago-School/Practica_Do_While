import random
def mostrar_letra_natanael():
    letra = """
    yo soy el f
    el f
    el f
    soy el f
    el f
    el f
    pa' que lo sepas
    el f
    el f
    si quieres probar
    yo soy el f
    el f
    el f
    y no se va a acabar
    yo soy el f
    el f
    el f
    pa' que lo sepas
    """
    print(letra)

def mostrar_letra_bad_bunny():
    letra = """
    tengo una neverita
    llena de cervezas
    la noche es larga
    y yo tengo prisa
    nunca me rindo
    no me voy a ir
    porque la fiesta apenas comienza
    """
    print(letra)

numero_secreto = random.randint(1, 10)
intento = None

while True:
    intento_str = input("adivina el numero entre 1 y 10: ")
    if intento_str == "":
        mostrar_letra_bad_bunny()
        break
    try:
        intento = int(intento_str)
        if intento == numero_secreto:
            print("correcto! has adivinado el numero.")
            break
        else:
            print("intenta de nuevo.")
            mostrar_letra_natanael()
    except ValueError:
        print("por favor ingresa un numero valido.")

![image](https://github.com/user-attachments/assets/cee20f7e-1929-49d3-aef6-ff8f3d15b84b)

