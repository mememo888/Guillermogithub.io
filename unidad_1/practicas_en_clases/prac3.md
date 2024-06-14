import random
nombre="Oso Polar"
saludos=[
    "Bienvenido "+nombre+", te saluda BDS",
    "Hola "+nombre+", en que puedo servir?",
    "Es un placer tenerte nuevamete "+nombre,
    "Hola "+nombre+", ¿cómo estás?",
    "Hola "+nombre+", ¿cómo te va?"
]
indice=random.randint(0,len(saludos)-1)
print(saludos[indice])