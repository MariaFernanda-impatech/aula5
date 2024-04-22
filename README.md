# aula5

num1 = 0.0
num2 = 0.0
num3 = 0.0
lista = [-2.0, -1.0, -0.5, 0.0, 0.5, 1.0, 2.0]

def funcao1 (num1):
	print("Dada a função f(x) = 2x⁴ - 2x² -x + 3, vamos calcular a função para alguns valores \n")
	final = 2*num1**4 - 2*num1**2 - num1 + 3
	print(f"Para x = {num1}, f(x) = {final}")
	
def funcao2 (num2):
	print("\n Dada a função g(x) = 5x/3^x - 1.1x^x, vamos calcular a função para alguns valores\n ")
	final = 5*num2/(3**num2) - 1.1*num2**num2
	print(f"Para x = {num2}, f(x) = {final}")

def funcao3 (num3):
	print("\n Dada a função h(x) = 2x² se x <=0 \n x/2 se 0<x<1 \n 1 se x = 1 \n e x + 1/2 se x >1, vamos calcular a função para alguns valores \n")
	if num3 <= 0:
		final = 2*num3**2
	elif num3 < 1:
		final = num3/2
	elif num3 == 1:
		final = 1
	else:
		final = num3 + 1/2
	print(f"Para x = {num3}, f(x) = {final} ")

def resultado_final (num1, num2, num3, lista):
	for i in range(len(lista)):
		num1 = lista[i]
		num2 = lista [i]
		num3 = lista [i]
		funcao1 (num1)
		funcao2 (num2)
		funcao3 (num3)

resultado_final (num1, num2, num3, lista)
