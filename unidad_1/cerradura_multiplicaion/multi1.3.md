#decalracion de variables y el ingreso de dos numeros 
num1 = float(input("dame un numero: "))
#decalracion de variables y el ingreso de dos numeros 
num2 = float(input("dame otro numero: "))

if num1 > num2:
    print("el primer numero ({}) es mayor que ({})")
elif num1 < num2:
    print("el segundo numero ({}) es mayor que ({})")
else:
    print("ambos son iguales")