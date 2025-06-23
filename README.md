# calculadora
Calculadora em Python/Tkinter

---

# 🧮 Calculadora Simples com Python e Tkinter

## ✨ Sobre o projeto

Este é um projetinho bem prático de **calculadora com interface gráfica**, desenvolvido usando o módulo `tkinter` do Python. É aquela ferramenta básica, mas que já dá uma boa noção de como construir GUIs (interfaces gráficas) no Python, além de reforçar conceitos de funções e manipulação de eventos.

Aqui você pode realizar as quatro operações matemáticas básicas:

* ✅ Soma
* ✅ Subtração
* ✅ Multiplicação
* ✅ Divisão

Tudo isso através de uma janelinha bonitinha, sem precisar usar terminal.

---

## 🚀 Como funciona o código?

### 🔧 As funções matemáticas

Logo no começo, o código define quatro funções bem simples que fazem os cálculos:

```python
def somar(a, b):
    return a + b
```

E segue assim para subtrair, multiplicar e dividir. No caso da divisão, tem uma proteção contra divisão por zero:

```python
def dividir(a, b):
    if b == 0:
        return "Divisão inválida"
    return a / b
```

### 🎛️ A interface gráfica

A interface é construída com `tkinter`:

* Tem dois campos de entrada (`Entry`) para você digitar os números.
* Um grupo de botões (`Radiobutton`) para escolher a operação desejada.
* Um botão (`Button`) chamado "Calcular" que, quando clicado, faz o cálculo baseado na operação escolhida.
* E, claro, um `Label` para exibir o resultado.

### 🧠 A lógica do cálculo

Quando você clica no botão, ele executa a função `calcular()`:

1. Primeiro, ele pega os valores digitados e tenta converter para `float`. Se der erro (tipo, você digitou texto), aparece uma janelinha de erro usando `messagebox.showerror()`.

2. Depois verifica qual operação foi selecionada pelos `Radiobuttons`.

3. Faz o cálculo correspondente chamando a função certa (somar, subtrair, multiplicar ou dividir).

4. Atualiza o `Label` mostrando o resultado formatadinho, no estilo:

```
Resultado: 5.0 + 3.0 = 8.0
```

### 🪟 A janela

---

## 📦 Como rodar

1. Clone o repositório ou copie o código.

2. Rode diretamente com Python 3:

```bash
python nome_do_arquivo.py
```

> Obs.: `tkinter` já vem embutido na maioria das instalações do Python, então não precisa instalar nada extra.

---

## 🏗 Melhorias que podem ser feitas

* 🎨 Melhorar o layout (usar `grid()` em vez de `pack()`).
* 💡 Adicionar operações mais avançadas (potência, raiz, etc.).
* 🗑️ Adicionar botão "Limpar".
* 😎 Aplicar temas (dark mode, por exemplo).

---

## 🤝 Contribuição

Esse projeto é simples, mas se quiser melhorar, fique à vontade para abrir uma issue ou fazer um pull request!

---
