# Calculadora com Funções em Python

Programa em Python que implementa uma **calculadora interativa**, organizada em **funções** para cada operação matemática.  
Esse formato deixa o código mais **limpo, modular e reutilizável**.

## 🚀 Código principal
```python
def soma(a, b):
    return a + b

def subtracao(a, b):
    return a - b

def multiplicacao(a, b):
    return a * b

def divisao(a, b):
    if b == 0:
        return "Erro: divisão por zero"
    return a / b

print("=== Calculadora com Funções ===")

while True:
    print("\nEscolha uma operação:")
    print("1 - Soma")
    print("2 - Subtração")
    print("3 - Multiplicação")
    print("4 - Divisão")
    print("0 - Sair")

    opcao = input("Digite a opção desejada: ")

    if opcao == "0":
        print("Encerrando a calculadora... Até logo!")
        break

    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))

    if opcao == "1":
        print("Resultado:", soma(num1, num2))
    elif opcao == "2":
        print("Resultado:", subtracao(num1, num2))
    elif opcao == "3":
        print("Resultado:", multiplicacao(num1, num2))
    elif opcao == "4":
        print("Resultado:", divisao(num1, num2))
    else:
        print("Opção inválida!")


O que foi aprendido
Criação de funções com def.
Uso de parâmetros e return.
Organização do código em blocos reutilizáveis.
Refatoração de código para maior clareza.
Boas práticas de modularização.

💭 Comentário pessoal

Foi muito interessante ver como funções deixam o programa mais organizado.
Antes a calculadora tinha muito código repetido, mas agora cada operação está em uma função separada.
Isso me ajudou a entender que funções são como “peças de LEGO” que posso combinar para montar programas maiores.
