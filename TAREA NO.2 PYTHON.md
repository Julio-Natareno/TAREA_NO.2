numero = int(input("Ingrese un número entero positivo: "))


print("Elija el tipo de triángulo:")
print("1. Triángulo  derecho")
print("2. Triángulo  izquierdo")
print("3. Triángulo  inferior")
print("4. Triángulo  superior")
opcion = int(input())


if opcion >= 1 and opcion <= 4:
    if opcion == 1:
        for i in range(1, numero + 1):
            print("* " * i)
    elif opcion == 2:
        for i in range(1, numero + 1):
            print("* " * (numero - i + 1))
    elif opcion == 3:
        for i in range(1, numero + 1):
            print("  " * (numero - i) + "* " * i)
    elif opcion == 4:
        for i in range(1, numero + 1):
            print("  " * (i - 1) + "* " * (numero - i + 1))
else:
    print("NO VALIDO.")