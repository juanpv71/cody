# cody
import random
print("¡Bienvenido al juego de adivinar el número!")
maximo = int(input("¿Hasta qué número quieres que piense el programa? "))
numero_secreto = random.randint(1, maximo)
intentos = 0
print(f"Estoy pensando en un número entre 1 y {maximo}...")
while True:
    intento = int(input("Adivina el número: "))
    intentos += 1

    if intento < numero_secreto:
        print("Demasiado bajo.")
    elif intento > numero_secreto:
        print("Demasiado alto.")
    else:
        print(f"🎉 ¡Correcto! Lo adivinaste en {intentos} intentos.")
        break
