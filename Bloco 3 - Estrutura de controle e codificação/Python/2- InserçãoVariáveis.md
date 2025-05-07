### 1. **Inserir valores em variáveis do tipo inteiro (int)**

Você pode simplesmente atribuir um valor inteiro a uma variável. Para inserir um valor em uma variável inteira, basta fazer o seguinte:

```python
idade = 25  # Inserindo o valor 25 na variável 'idade'
numero_de_filhos = 2  # Inserindo o valor 2 na variável 'numero_de_filhos'
```

Caso você queira obter um valor inteiro de um usuário, você pode usar a função `input()` e converter a entrada para um número inteiro:

```python
idade = int(input("Digite sua idade: "))  # O valor inserido pelo usuário será convertido para inteiro
print(idade)
```

### 2. **Inserir valores em variáveis do tipo ponto flutuante (float)**

Para variáveis do tipo `float`, o processo é similar, mas o valor precisa ser um número com ponto decimal. Veja como fazer isso:

```python
altura = 1.75  # Inserindo o valor 1.75 na variável 'altura'
peso = 70.5    # Inserindo o valor 70.5 na variável 'peso'
```

Se você deseja obter um valor decimal do usuário:

```python
altura = float(input("Digite sua altura em metros: "))  # O valor inserido será convertido para float
print(altura)
```

### 3. **Inserir valores em variáveis do tipo string (str)**

Para variáveis do tipo `str` (strings ou textos), você pode atribuir diretamente uma string, ou pode obter a entrada do usuário:

```python
nome = "Maria"  # Atribuindo um texto à variável 'nome'
cidade = "São Paulo"  # Atribuindo um texto à variável 'cidade'
```

Se você quer que o usuário insira um valor de texto:

```python
nome = input("Digite seu nome: ")  # O valor inserido será armazenado como uma string
print(nome)
```

### 4. **Inserir valores em variáveis do tipo booleano (bool)**

O tipo booleano (`bool`) só pode ter dois valores: `True` (verdadeiro) ou `False` (falso). Para inserir um valor booleano, você pode atribuir diretamente:

```python
esta_chovendo = True  # Atribuindo o valor True
sol = False  # Atribuindo o valor False
```

Para obter um valor booleano do usuário, você pode usar `input()` e comparar o valor inserido com uma string específica (como "sim" ou "não"):

```python
resposta = input("Está chovendo? (sim/nao): ").lower()  # Pegando o valor e transformando para minúsculas
if resposta == "sim":
    esta_chovendo = True
else:
    esta_chovendo = False
print(esta_chovendo)
```

### 5. **Inserir valores em variáveis do tipo lista (list)**

Para listas, você pode simplesmente atribuir uma lista de elementos a uma variável:

```python
frutas = ["maçã", "banana", "laranja"]  # Atribuindo uma lista de frutas à variável 'frutas'
```

Para obter uma lista do usuário (por exemplo, se o usuário quiser inserir várias frutas), você pode usar um laço para coletar as entradas:

```python
frutas = []
quantidade = int(input("Quantas frutas você quer adicionar? "))
for i in range(quantidade):
    fruta = input(f"Digite a fruta #{i+1}: ")  # Obtendo o nome de cada fruta
    frutas.append(fruta)  # Adicionando a fruta à lista
print(frutas)
```

### 6. **Inserir valores em variáveis do tipo dicionário (dict)**

Dicionários armazenam pares de chave e valor. Você pode atribuir diretamente um dicionário ou inserir elementos com a função `input()`:

```python
pessoa = {"nome": "Maria", "idade": 30}  # Atribuindo um dicionário com chaves e valores
```

Para obter dados de um usuário e inserir em um dicionário:

```python
pessoa = {}
pessoa["nome"] = input("Digite seu nome: ")  # Inserindo a chave "nome" e o valor fornecido pelo usuário
pessoa["idade"] = int(input("Digite sua idade: "))  # Inserindo a chave "idade" e o valor fornecido
print(pessoa)
```

### 7. **Inserir valores em variáveis do tipo tupla (tuple)**

As tuplas são imutáveis, ou seja, uma vez criadas, você não pode mudar seus valores. Porém, ao criar uma tupla, você pode inserir os valores diretamente:

```python
coordenadas = (10, 20)  # Inserindo uma tupla com dois números
```

Se quiser criar uma tupla a partir de entradas do usuário, você pode fazer assim:

```python
x = int(input("Digite a coordenada X: "))
y = int(input("Digite a coordenada Y: "))
coordenadas = (x, y)  # Criando uma tupla com as coordenadas inseridas
print(coordenadas)
```

### 8. **Inserir valores em variáveis do tipo conjunto (set)**

Os conjuntos não permitem elementos duplicados. Você pode adicionar valores diretamente ou coletá-los do usuário:

```python
frutas_unicas = {"maçã", "banana", "laranja"}  # Conjunto com elementos únicos
```

Para obter dados do usuário e inserir em um conjunto:

```python
frutas_unicas = set()  # Criando um conjunto vazio
quantidade = int(input("Quantas frutas você quer adicionar? "))
for i in range(quantidade):
    fruta = input(f"Digite a fruta #{i+1}: ")
    frutas_unicas.add(fruta)  # Adicionando uma fruta ao conjunto
print(frutas_unicas)
```

### Resumo

* **Inteiros (int)**: Use números sem ponto decimal, como `idade = 25`.
* **Flutuantes (float)**: Use números com ponto decimal, como `altura = 1.75`.
* **Strings (str)**: Use texto entre aspas, como `nome = "Maria"`.
* **Booleanos (bool)**: Use `True` ou `False`, como `esta_chovendo = True`.
* **Listas (list)**: Use colchetes para armazenar vários itens, como `frutas = ["maçã", "banana"]`.
* **Dicionários (dict)**: Use chaves e valores, como `pessoa = {"nome": "Maria", "idade": 30}`.
* **Tuplas (tuple)**: Use parênteses para armazenar dados imutáveis, como `coordenadas = (10, 20)`.
* **Conjuntos (set)**: Use chaves para armazenar elementos únicos, como `frutas_unicas = {"maçã", "banana"}`.

