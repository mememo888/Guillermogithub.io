import numpy as np
import matplotlib.pyplot as plt

# Función para resolver la ecuación cuadrática
def resolver_cuadratica(a, b, c):
    if a > 0 and 4*a*c > b**2:
        # Calculamos el discriminante
        discriminante = b**2 - 4*a*c
        # Calculamos las dos soluciones
        sol1 = (-b - np.sqrt(discriminante)) / (2*a)
        sol2 = (-b + np.sqrt(discriminante)) / (2*a)
        return sol1, sol2
    else:
        return "Las condiciones no se cumplen"

# Coeficientes de la ecuación cuadrática
a = 1  # a debe ser mayor que 0
b = 2
c = 1  # 4ac debe ser mayor que b^2

# Resolvemos la ecuación
soluciones = resolver_cuadratica(a, b, c)

# Verificamos si se obtuvieron soluciones
if isinstance(soluciones, tuple):
    # Creamos valores para x
    x = np.linspace(-10, 10, 400)
    # Calculamos los valores de y usando la ecuación cuadrática
    y = a*x**2 + b*x + c

    # Graficamos la función
    plt.figure()
    plt.plot(x, y, label=f'${{a}}x^2 + {b}x + {c}$')
    # Marcamos las soluciones en el gráfico
    plt.scatter([soluciones[0], soluciones[1]], [0, 0], color='red')
    plt.title('Gráfico de la Ecuación Cuadrática')
    plt.xlabel('x')
    plt.ylabel('y')
    plt.legend()
    plt.grid(True)
    plt.axhline(0, color='black',linewidth=0.5)
    plt.axvline(0, color='black',linewidth=0.5)
    plt.show()
else:
    print(soluciones)
