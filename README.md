# Secuencia de Fibonacci  

En este código ingresas la cantidad de números que quieres que genere la secuencia de Fibonacci.  

```python
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
