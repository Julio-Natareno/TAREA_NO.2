Algoritmo triangulo 
	numero = leer("Ingrese un n�mero entero positivo: ")
	opcion = leer("Elija el tipo de tri�ngulo:\n1. Tri�ngulo derecho\n2. Tri�ngulo izquierdo\n3. Tri�ngulo inferior\n4. Tri�ngulo superior\n")
	
	numero = convertir(numero, entero)
	opcion = convertir(opcion, entero)
	
	si opcion >= 1 y opcion <= 4 entonces
		si opcion == 1 entonces
			para i desde 1 hasta numero hacer
				imprimir("* " * i)
			finpara
		sino si opcion == 2 entonces
				para i desde 1 hasta numero hacer
					imprimir("  " * (numero - i) + "* " * i)
				finpara
			sino si opcion == 3 entonces
					para i desde 1 hasta numero hacer
						imprimir("* " * (numero - i + 1))
					finpara
				sino si opcion == 4 entonces
						para i desde 1 hasta numero hacer
							imprimir("  " * (i - 1) + "* " * (numero - i + 1))
						finpara
					sino
						imprimir("Opci�n no v�lida.")
					finsi
				sino
					imprimir("N�mero no v�lido.")
finSi

FinAlgoritmo
