Vamos aprender sobre **estruturas de decisão** em Python, que são usadas para **tomar decisões** no código, ou seja, para executar diferentes blocos de código dependendo de certas condições.

### 1. **Estrutura `if` (Se)**

A estrutura `if` é usada para **verificar uma condição** e, se essa condição for verdadeira, executa um bloco de código. Caso contrário, o código dentro do bloco `if` será ignorado.

#### Sintaxe básica:

```python
if condição:
    # Código a ser executado se a condição for verdadeira
```

#### Exemplo:

```python
idade = 18

if idade >= 18:
    print("Você é maior de idade!")  # Será executado porque a condição é verdadeira
```

Neste exemplo, a condição `idade >= 18` é verdadeira, então a mensagem "Você é maior de idade!" será impressa.

### 2. **Estrutura `else` (Senão)**

O `else` é usado junto com o `if` para **executar um bloco de código quando a condição do `if` for falsa**.

#### Sintaxe básica:

```python
if condição:
    # Código a ser executado se a condição for verdadeira
else:
    # Código a ser executado se a condição for falsa
```

#### Exemplo:

```python
idade = 16

if idade >= 18:
    print("Você é maior de idade!")
else:
    print("Você é menor de idade!")  # Será executado porque a condição do 'if' é falsa
```

Neste exemplo, como a condição `idade >= 18` é falsa, o código dentro do `else` será executado, e "Você é menor de idade!" será impresso.

### 3. **Estrutura `elif` (Senão, se)**

O `elif` é uma combinação de **`else` + `if`**, e é usado quando você quer **verificar múltiplas condições**. Caso a primeira condição seja falsa, ele verifica a condição do `elif`. Você pode ter vários `elif` seguidos, e o primeiro que for verdadeiro será executado.

#### Sintaxe básica:

```python
if condição1:
    # Código a ser executado se condição1 for verdadeira
elif condição2:
    # Código a ser executado se condição2 for verdadeira
else:
    # Código a ser executado se todas as condições forem falsas
```

#### Exemplo:

```python
idade = 20

if idade < 13:
    print("Você é uma criança.")
elif idade < 18:
    print("Você é um adolescente.")  # Vai ser executado porque a condição é verdadeira
else:
    print("Você é um adulto.")
```

Neste exemplo:

* A primeira condição `idade < 13` é falsa.
* A segunda condição `idade < 18` é verdadeira, então a mensagem "Você é um adolescente." será impressa.
* O `else` não será executado porque já houve uma condição verdadeira.

### 4. **Estruturas compostas**

Você pode combinar múltiplas condições em uma estrutura de decisão. Isso é feito usando operadores lógicos como **`and`**, **`or`** e **`not`**.

#### Operadores Lógicos:

* **`and`**: Verifica se **ambas as condições** são verdadeiras.
* **`or`**: Verifica se **pelo menos uma** das condições é verdadeira.
* **`not`**: Inverte o valor da condição (se a condição for `True`, ela se torna `False`, e vice-versa).

#### Exemplo com `and`:

```python
idade = 20
tem_diploma = True

if idade >= 18 and tem_diploma:
    print("Você pode se inscrever no curso.")
else:
    print("Você não pode se inscrever no curso.")
```

Neste caso, as duas condições precisam ser verdadeiras para o código dentro do `if` ser executado. O programa vai verificar se a `idade` é maior ou igual a 18 **e** se a pessoa tem diploma.

#### Exemplo com `or`:

```python
idade = 16
tem_permissao = True

if idade >= 18 or tem_permissao:
    print("Você pode entrar na festa.")
else:
    print("Você não pode entrar na festa.")
```

Neste caso, **se qualquer uma das condições for verdadeira**, o bloco do `if` será executado. O programa vai verificar se a `idade` é maior ou igual a 18 **ou** se a pessoa tem permissão para entrar na festa.

#### Exemplo com `not`:

```python
idade = 30

if not idade < 18:  # Verifica se idade NÃO é menor que 18
    print("Você é maior de idade!")
else:
    print("Você é menor de idade.")
```

Aqui, `not idade < 18` inverte a condição, ou seja, ele vai verificar se a pessoa **não** é menor de idade (ou seja, é maior de 18).

### 5. **Estrutura de decisão aninhada**

Você também pode **anidar estruturas de decisão** dentro de outras. Isso é útil quando você tem condições mais complexas.

#### Exemplo:

```python
idade = 22
tem_diploma = True

if idade >= 18:
    if tem_diploma:
        print("Você pode se inscrever no curso.")
    else:
        print("Você precisa de um diploma para se inscrever no curso.")
else:
    print("Você precisa ter 18 anos ou mais para se inscrever no curso.")
```

Neste caso, o programa verifica primeiro se a `idade` é maior ou igual a 18. Se for, ele verifica se a pessoa tem diploma. Dependendo dos resultados, ele imprime mensagens diferentes.

### Resumo das estruturas de decisão:

* **`if`**: Verifica se uma condição é verdadeira.
* **`else`**: Executa um código quando a condição do `if` for falsa.
* **`elif`**: Permite testar várias condições, caso a do `if` seja falsa.
* **Operadores lógicos (`and`, `or`, `not`)**: Permitem combinar ou inverter condições.
* **Estruturas aninhadas**: Você pode colocar uma estrutura `if` dentro de outra.

