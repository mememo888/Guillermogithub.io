#sera el uso de operacion de la suma 
print("cerradura: la suma de doa numeros rales siempre da como resultado otro numero real")
print("a + b pertenece R")
print()

print("el siguiente programa realizara la propiedad de cerradura")
print()

num1 = float(input("dame un numero: "))
#decalracion de variables y el ingreso de dos numeros 
num2 = float(input("dame otro numero: "))

suma = num1 + num2

#el i.integer es para el true o false 
if suma.is_integer():
    resultado = "entero"
else:
    resultado = "racinal"

print()
print("el resultado de la suma es: ", suma)
print("el resultado de la operacion es de: ", resultado)