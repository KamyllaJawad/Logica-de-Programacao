# Comandos básicos em Python

### 1. **`print()` - Exibindo informações na tela**

O comando `print()` é utilizado para **mostrar** informações na tela, como texto, valores de variáveis, ou resultados de expressões.

#### Exemplo:

```python
print("Olá, Mundo!")  # Vai imprimir "Olá, Mundo!" na tela
```

Você pode usar o `print()` para imprimir variáveis e resultados de cálculos:

```python
nome = "João"
idade = 25

print(nome)  # Vai imprimir "João"
print(idade)  # Vai imprimir 25
print("A idade de", nome, "é", idade)  # Vai imprimir "A idade de João é 25"
```

Também pode imprimir cálculos diretamente:

```python
soma = 5 + 3
print(soma)  # Vai imprimir 8
```

Você também pode formatar a saída com f-strings (disponível a partir do Python 3.6):

```python
print(f"A idade de {nome} é {idade}")  # Vai imprimir "A idade de João é 25"
```

### 2. **`input()` - Recebendo entradas do usuário**

O comando `input()` é utilizado para **receber dados** do usuário. Ele mostra uma mensagem na tela e aguarda que o usuário digite algo. O valor que o usuário digitar é retornado como **uma string** (texto).

#### Exemplo:

```python
nome = input("Digite seu nome: ")
print(f"Olá, {nome}!")  # Vai saudar o usuário com o nome digitado
```

Se você quiser **converter** o valor digitado para outro tipo de dado, como número, você pode usar funções como `int()` (para inteiros) ou `float()` (para números decimais):

```python
idade = int(input("Digite sua idade: "))  # Converte a entrada para um número inteiro
print(f"Você tem {idade} anos.")
```

### 3. **`len()` - Tamanho de uma string ou lista**

O comando `len()` retorna o **tamanho** de uma string ou de uma lista, ou seja, quantos caracteres ou itens ela tem.

#### Exemplo:

```python
nome = "Maria"
tamanho_nome = len(nome)
print(f"O nome {nome} tem {tamanho_nome} caracteres.")  # Vai imprimir "O nome Maria tem 5 caracteres"
```

Com listas:

```python
numeros = [1, 2, 3, 4, 5]
tamanho_lista = len(numeros)
print(f"A lista tem {tamanho_lista} itens.")  # Vai imprimir "A lista tem 5 itens."
```

### 4. **`type()` - Tipo de dado**

O comando `type()` é utilizado para verificar o **tipo** de uma variável ou valor. Isso é útil para saber se a variável é uma string, número, lista, etc.

#### Exemplo:

```python
numero = 10
texto = "Olá"
lista = [1, 2, 3]

print(type(numero))  # Vai imprimir <class 'int'> (inteiro)
print(type(texto))   # Vai imprimir <class 'str'> (string)
print(type(lista))   # Vai imprimir <class 'list'> (lista)
```

### 5. **`int()` e `float()` - Conversão de tipos**

Você pode usar `int()` e `float()` para **converter valores** de um tipo para outro. O `int()` converte para inteiro e o `float()` converte para número decimal.

#### Exemplo:

```python
numero_str = "10"
numero_int = int(numero_str)  # Converte de string para inteiro
print(numero_int)  # Vai imprimir 10

numero_str_decimal = "3.14"
numero_float = float(numero_str_decimal)  # Converte de string para float
print(numero_float)  # Vai imprimir 3.14
```

### 6. **`str()` - Converter para string**

O comando `str()` converte qualquer tipo de dado para **string**. Isso é útil quando você precisa concatenar números com texto, por exemplo.

#### Exemplo:

```python
idade = 25
nome = "João"

# Para concatenar uma string com um número, precisamos converter o número para string
print("A idade de " + nome + " é " + str(idade))  # Vai imprimir "A idade de João é 25"
```

### 7. **`sum()` - Somando elementos**

O comando `sum()` é utilizado para somar os elementos de uma **lista** ou **tupla** de números.

#### Exemplo:

```python
numeros = [1, 2, 3, 4, 5]
soma = sum(numeros)
print(f"A soma dos números é: {soma}")  # Vai imprimir "A soma dos números é: 15"
```

### 8. **`max()` e `min()` - Máximo e Mínimo**

Os comandos `max()` e `min()` são usados para **encontrar o maior ou o menor valor** em uma lista ou tupla.

#### Exemplo:

```python
numeros = [1, 2, 3, 4, 5]

maior = max(numeros)  # Encontra o maior valor
menor = min(numeros)  # Encontra o menor valor

print(f"O maior número é {maior}")  # Vai imprimir "O maior número é 5"
print(f"O menor número é {menor}")  # Vai imprimir "O menor número é 1"
```

### 9. **`round()` - Arredondar números**

O comando `round()` arredonda um número para o número de casas decimais que você especificar.

#### Exemplo:

```python
numero = 3.14159
numero_arredondado = round(numero, 2)  # Arredonda para 2 casas decimais
print(numero_arredondado)  # Vai imprimir 3.14
```

### 10. **`input()` com múltiplas entradas**

Se você precisar obter **várias entradas** de uma vez, pode fazer isso dentro de um loop ou pedindo ao usuário para separar as entradas por um delimitador, como uma vírgula.

```python
entradas = input("Digite seus números separados por vírgula: ")
lista_numeros = entradas.split(",")  # Divida a entrada em uma lista
lista_numeros = [int(num) for num in lista_numeros]  # Converte cada item para inteiro

print(lista_numeros)
```

### Resumo dos Comandos:

* **`print()`**: Exibe informações na tela.
* **`input()`**: Recebe dados do usuário.
* **`len()`**: Retorna o tamanho de uma string ou lista.
* **`type()`**: Verifica o tipo de uma variável.
* **`int()`** e **`float()`**: Convertem valores para inteiro ou decimal, respectivamente.
* **`str()`**: Converte qualquer tipo de dado para string.
* **`sum()`**: Soma os elementos de uma lista ou tupla.
* **`max()`** e **`min()`**: Encontram o maior e o menor valor, respectivamente.
* **`round()`**: Arredonda um número para um número específico de casas decimais.

