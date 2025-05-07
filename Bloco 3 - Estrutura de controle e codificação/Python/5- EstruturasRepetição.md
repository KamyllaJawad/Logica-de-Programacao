Vamos aprender sobre **estruturas de repetição** em Python, que são usadas para executar um bloco de código várias vezes. As duas principais estruturas de repetição em Python são o **`for`** e o **`while`**. 

### 1. **Estrutura `for`**

A estrutura `for` é usada quando você sabe **quantas vezes** quer repetir uma ação. Ela geralmente é usada para percorrer itens dentro de uma lista, tupla, string, ou até mesmo intervalos de números.

#### 1.1 **Repetindo com uma lista**

Se você tem uma lista de itens e quer fazer algo com cada item, pode usar o `for` assim:

```python
frutas = ["maçã", "banana", "laranja"]

for fruta in frutas:
    print(f"A fruta é: {fruta}")
```

**Explicação**: A cada repetição, o valor de `fruta` será um item da lista `frutas`. Na primeira repetição, `fruta` será `"maçã"`, na segunda repetição será `"banana"`, e assim por diante. O resultado será:

```
A fruta é: maçã
A fruta é: banana
A fruta é: laranja
```

#### 1.2 **Repetindo com `range()`**

Se você não tem uma lista, mas quer repetir um bloco de código um número específico de vezes, pode usar o `range()`. O `range()` cria uma sequência de números, e o `for` pode percorrer esses números.

```python
for i in range(5):  # Vai repetir 5 vezes
    print(f"Repetição {i + 1}")
```

**Explicação**: O `range(5)` cria uma sequência de números de 0 a 4 (5 números no total), e o `for` repete o código dentro do bloco 5 vezes. O resultado será:

```
Repetição 1
Repetição 2
Repetição 3
Repetição 4
Repetição 5
```

Você também pode definir o início e o final da sequência com o `range()`:

```python
for i in range(2, 10):  # Começa de 2 e vai até 9
    print(i)
```

Isso vai imprimir os números de 2 a 9:

```
2
3
4
5
6
7
8
9
```

Você pode até usar um passo maior no `range()`:

```python
for i in range(0, 10, 2):  # Vai de 0 a 9, pulando de 2 em 2
    print(i)
```

Isso vai imprimir:

```
0
2
4
6
8
```

### 2. **Estrutura `while`**

A estrutura `while` é usada quando você quer repetir um bloco de código enquanto uma **condição** for verdadeira. Ou seja, o `while` continua executando o código enquanto a condição for válida.

#### 2.1 **Repetindo com `while`**

```python
contador = 0

while contador < 5:
    print(f"Contagem: {contador}")
    contador += 1  # Incrementa 1 a cada repetição
```

**Explicação**: O código vai continuar rodando enquanto `contador` for menor que 5. O valor de `contador` é incrementado em 1 a cada repetição. O resultado será:

```
Contagem: 0
Contagem: 1
Contagem: 2
Contagem: 3
Contagem: 4
```

Se a condição for falsa no início, o código dentro do `while` **não** será executado. Por exemplo:

```python
contador = 10

while contador < 5:
    print(f"Contagem: {contador}")
    contador += 1
```

Neste caso, o código **não será executado** porque `contador` já começa com 10, e a condição `contador < 5` é falsa.

#### 2.2 **Usando `break` e `continue` no `while`**

O `while` também pode ser controlado com os comandos `break` e `continue`:

* **`break`**: Sai do laço, interrompendo a repetição.
* **`continue`**: Pula a iteração atual e vai para a próxima.

Exemplo de **`break`**:

```python
contador = 0

while True:  # Isso cria um laço infinito
    if contador == 5:
        break  # Quando contador atingir 5, o laço será interrompido
    print(f"Contagem: {contador}")
    contador += 1
```

O resultado será:

```
Contagem: 0
Contagem: 1
Contagem: 2
Contagem: 3
Contagem: 4
```

Exemplo de **`continue`**:

```python
contador = 0

while contador < 5:
    contador += 1
    if contador == 3:
        continue  # Quando contador for 3, o código abaixo será ignorado e a repetição continua
    print(f"Contagem: {contador}")
```

O resultado será:

```
Contagem: 1
Contagem: 2
Contagem: 4
Contagem: 5
```

Quando `contador` é 3, o comando `continue` faz com que o código pule o `print()` e vá para a próxima iteração.

### 3. **Usando `for` e `while` juntos**

Às vezes, você pode querer usar `for` e `while` juntos, ou até mesmo aninhá-los (um dentro do outro), dependendo do que está tentando fazer.

Exemplo com `for` dentro de um `while`:

```python
contador = 0

while contador < 3:
    print(f"Contagem do while: {contador}")
    for i in range(3):  # Um 'for' dentro do 'while'
        print(f"  Contagem do for: {i}")
    contador += 1
```

Isso vai imprimir:

```
Contagem do while: 0
  Contagem do for: 0
  Contagem do for: 1
  Contagem do for: 2
Contagem do while: 1
  Contagem do for: 0
  Contagem do for: 1
  Contagem do for: 2
Contagem do while: 2
  Contagem do for: 0
  Contagem do for: 1
  Contagem do for: 2
```

### 4. **Conclusão**

* **`for`**: Quando você sabe quantas vezes vai repetir o código.
* **`while`**: Quando você quer repetir o código até que uma condição seja falsa.
* Você pode usar **`break`** para sair do laço e **`continue`** para pular para a próxima iteração.
