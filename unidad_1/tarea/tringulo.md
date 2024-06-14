import math

def calcular_lado_faltante():
    print("Introduce los valores de dos lados que conoscas ")
    print("Deja en blaco el valor del lado que desas a calcular")

    a = input("Cateto a: ")
    b = input("cateto b: ")
    c = input("Hipotenusa c: ")

    a = float (a) if a else None
    b = float (b) if b else None
    c = float (c) if c else None

    if a is None and b is not None and c is not None:
        a = math.sqrt(c**2 - b**2)
        lado_calculado = "a (cateto)"

    if b is None and a is not None and c is not None:
        b = math.sqrt(c**2 - a**2)
        lado_calculado = "b (cateto)"

    if c is None and a is not None and b is not None:
        c = math.sqrt(a**2 + b**2)
        lado_calculado = "c (hipotenusa)"

    else:
            return "Error: debe porporcionar bien los lados"

    return f"El lado faltante es {lado_calculado} y su valor es {a if lado_calculado =='a (cateto)'else b if lado_calculado == 'b (cateto)' else c if lado_calculado == 'c (hipotenusa)'else Pylance}"

resultado = calcular_lado_faltante()
print(resultado)