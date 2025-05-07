### O que são variáveis?

Variáveis são como "caixas" que armazenam dados (valores). Você pode dar qualquer nome para uma variável e armazenar informações nela. Essas informações podem ser de diferentes tipos, como números, textos, listas e muito mais.

### Tipos de dados em Python

#### 1. **Inteiros (int)**

São números inteiros, sem ponto decimal.

Exemplo:

```python
idade = 25  # Aqui, 'idade' é uma variável do tipo inteiro.
numero_de_filhos = 2  # Outra variável inteira.
```

Você pode fazer operações com números inteiros, como soma, subtração, multiplicação e divisão.

```python
resultado = idade + numero_de_filhos  # Soma
print(resultado)  # Vai imprimir 27
```

#### 2. **Ponto flutuante (float)**

São números com ponto decimal.

Exemplo:

```python
altura = 1.75  # 'altura' é uma variável do tipo float.
peso = 70.5  # 'peso' também é um float.
```

Você também pode fazer operações com floats:

```python
imc = peso / (altura ** 2)  # Calculando o IMC
print(imc)  # Vai imprimir o resultado do cálculo
```

#### 3. **Strings (str)**

São sequências de caracteres, ou seja, textos. Strings podem ser criadas com aspas simples (`'`) ou duplas (`"`).

Exemplo:

```python
nome = "João"  # 'nome' é uma variável do tipo string.
cidade = 'São Paulo'  # Outra string.
```

Você pode usar operações com strings, como concatenar (juntar) elas:

```python
mensagem = nome + " mora em " + cidade  # Concatenando strings
print(mensagem)  # Vai imprimir "João mora em São Paulo"
```

#### 4. **Booleanos (bool)**

São valores lógicos, que podem ser **`True`** (verdadeiro) ou **`False`** (falso).

Exemplo:

```python
esta_chovendo = True  # 'esta_chovendo' é um booleano.
sol = False  # 'sol' é um booleano.
```

Você pode usar booleans para fazer decisões em seu código (com `if` e `else`):

```python
if esta_chovendo:
    print("Leve um guarda-chuva!")
else:
    print("Está ensolarado, aproveite o dia!")
```

#### 5. **Listas (list)**

Listas são coleções de valores. Esses valores podem ser de tipos diferentes e são armazenados entre colchetes (`[]`).

Exemplo:

```python
frutas = ["maçã", "banana", "laranja"]  # 'frutas' é uma lista de strings.
numeros = [10, 20, 30, 40]  # 'numeros' é uma lista de inteiros.
```

Você pode acessar os elementos de uma lista utilizando índices (o índice começa de 0):

```python
print(frutas[0])  # Vai imprimir "maçã"
```

Você também pode modificar um valor dentro da lista:

```python
frutas[1] = "uva"  # Substitui "banana" por "uva"
print(frutas)  # Vai imprimir ['maçã', 'uva', 'laranja']
```

#### 6. **Dicionários (dict)**

Dicionários armazenam dados em pares de chave e valor. Eles são definidos com chaves (`{}`), onde você tem uma chave e um valor associados.

Exemplo:

```python
pessoa = {"nome": "Maria", "idade": 30}  # 'pessoa' é um dicionário.
```

Você pode acessar os valores de um dicionário utilizando a chave:

```python
print(pessoa["nome"])  # Vai imprimir "Maria"
```

Você também pode adicionar ou modificar pares chave-valor:

```python
pessoa["cidade"] = "Rio de Janeiro"  # Adicionando uma nova chave "cidade"
print(pessoa)  # Vai imprimir {'nome': 'Maria', 'idade': 30, 'cidade': 'Rio de Janeiro'}
```

#### 7. **Tuplas (tuple)**

Tuplas são semelhantes a listas, mas são imutáveis, ou seja, uma vez criadas, não podem ser alteradas.

Exemplo:

```python
coordenadas = (10, 20)  # 'coordenadas' é uma tupla de inteiros.
```

Você pode acessar os elementos de uma tupla como uma lista:

```python
print(coordenadas[0])  # Vai imprimir 10
```

#### 8. **Conjuntos (set)**

Conjuntos são coleções de elementos únicos, ou seja, não permitem duplicatas. Eles são definidos com chaves (`{}`), assim como dicionários, mas sem chave/valor.

Exemplo:

```python
frutas_unicas = {"maçã", "banana", "laranja", "maçã"}  # 'frutas_unicas' é um conjunto.
print(frutas_unicas)  # Vai imprimir {'maçã', 'laranja', 'banana'}, sem duplicatas.
```

### Resumo

* **int**: Números inteiros (sem ponto decimal).
* **float**: Números com ponto decimal.
* **str**: Texto ou sequência de caracteres.
* **bool**: Valores lógicos, `True` ou `False`.
* **list**: Lista de valores.
* **dict**: Dicionário com pares chave/valor.
* **tuple**: Lista imutável.
* **set**: Conjunto de elementos únicos.

