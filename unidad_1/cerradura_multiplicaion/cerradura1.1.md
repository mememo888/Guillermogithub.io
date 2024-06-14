#sera el uso de operacion de la multiplicacion 
print("cerradura: la multiplicaion de doa numeros rales siempre da como resultado otro numero real")
print("a * b pertenece R")
print()

print("el siguiente programa realizara la propiedad de cerradura")
print()

num1 = float(input("dame un numero: "))
#decalracion de variables y el ingreso de dos numeros 
num2 = float(input("dame otro numero: "))

multiplicaion = num1 * num2

if multiplicaion.is_integer():
    resultado = "entero"
else:
    resultado = "racinal"

print()
print("el resultado de la multiplicaion es: ", multiplicaion)
print("el resultado de la operacion es de: ", resultado)
