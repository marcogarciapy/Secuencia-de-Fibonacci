# Secuencia-de-Fibonacci
En este codigo ingresas la cantidad de numeros los cuales quieres que haga la secuencia de Fibonacci

def fibonacci(n):
    a, b = 0, 1
    sequence = []
    for _ in range(n):
        sequence.append(a)
        a, b = b, a + b
    return sequence

num_terms = int(input("Ingrese el número de términos de la secuencia Fibonacci que desea: "))
fib_sequence = fibonacci(num_terms)
print(f"Secuencia Fibonacci con {num_terms} términos: {fib_sequence}")
