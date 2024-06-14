#este codigo crea in grafo dirigido con 4 variables 
#Creamos un grafo vacio
grafo = {}

#Agregamos vertices al grafos 
grafo['A'] = ['B', 'C']
grafo['B'] = ['D']
grafo['C'] = ['D']
grafo['D'] = []

print("grafo: ")

for vertice, adyacente in grafo.items():
    print(f"Vertice {vertice} -> {adyacente}")