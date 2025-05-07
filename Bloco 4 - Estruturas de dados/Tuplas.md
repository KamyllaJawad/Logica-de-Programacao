### O que são **tuplas**? 🧩

Uma **tupla** é uma **sequência ordenada** de elementos, **semelhante a uma lista**, mas com uma grande diferença: **as tuplas são imutáveis**. Ou seja, uma vez criada uma tupla, **você não pode modificar seus valores**.

### Características das tuplas:

* **Imutabilidade**: Você **não pode** alterar, adicionar ou remover elementos de uma tupla depois que ela for criada.
* **Ordenação**: Os elementos de uma tupla têm uma ordem específica e você pode acessar os itens pelo índice.
* **Armazenamento de diferentes tipos de dados**: Assim como as listas, tuplas podem armazenar diferentes tipos de dados, como números, strings, e até outras tuplas.

### Como criar uma tupla?

Em Python, você cria uma tupla utilizando **parênteses** `()`.

#### Exemplo básico de uma tupla:

```python
tupla = (1, 2, 3, 4, 5)
```

Aqui, temos uma tupla com 5 elementos: `1`, `2`, `3`, `4` e `5`. Ao contrário das listas, se tentarmos modificar um dos elementos da tupla, vamos obter um erro:

```python
tupla[0] = 10  # Isso geraria um erro porque tuplas são imutáveis
```

### 1. **Tupla com números**

Vamos ver como armazenar uma sequência de números em uma tupla e acessá-los.

```python
numeros = (10, 20, 30, 40, 50)

# Acessando o primeiro item (índice 0)
print(numeros[0])  # Vai imprimir 10

# Acessando o último item (índice -1)
print(numeros[-1])  # Vai imprimir 50
```

**Explicação**: Nesse exemplo, estamos criando uma tupla com 5 números. Usamos índices para acessar valores específicos da tupla. O índice `0` acessa o primeiro valor, enquanto o índice `-1` acessa o último valor.

---

### 2. **Tupla com diferentes tipos de dados**

Uma tupla pode armazenar diferentes tipos de dados, como números, strings e até listas!

```python
dados = ("João", 25, 1.75, ["Python", "Java", "C++"])

# Acessando a string
print(dados[0])  # Vai imprimir "João"

# Acessando o número
print(dados[1])  # Vai imprimir 25

# Acessando a lista dentro da tupla
print(dados[3])  # Vai imprimir ["Python", "Java", "C++"]

# Acessando um item dentro da lista
print(dados[3][1])  # Vai imprimir "Java"
```

**Explicação**: Aqui, temos uma tupla que contém uma **string**, um **número**, um **número decimal (float)** e uma **lista**. Usamos índices para acessar esses valores, e também podemos acessar os itens dentro da lista que está dentro da tupla.

---

### 3. **Tupla com uma única variável**

Se você quiser criar uma tupla com apenas **um elemento**, é preciso colocar uma vírgula após o valor, caso contrário, o Python não entenderá que você está criando uma tupla.

```python
tupla_unica = (10,)  # Essa é uma tupla com um único item
print(type(tupla_unica))  # Vai mostrar <class 'tuple'>

# Se você não colocar a vírgula, Python criará uma variável do tipo inteiro
nao_tupla = (10)
print(type(nao_tupla))  # Vai mostrar <class 'int'>
```

**Explicação**: Quando criamos uma tupla com um único elemento, é necessário colocar a vírgula `,` para que o Python entenda que se trata de uma tupla. Sem a vírgula, o Python interpreta como o tipo de dado do valor inserido (no caso, um **inteiro**).

---

### 4. **Tupla com fatiamento (slicing)**

Você pode acessar **sublistas** de uma tupla usando o fatiamento, o que significa pegar uma **parte** da tupla.

```python
tupla = (1, 2, 3, 4, 5, 6)

# Pegando do segundo até o quarto elemento (índices 1 até 3)
sub_tupla = tupla[1:4]
print(sub_tupla)  # Vai imprimir (2, 3, 4)

# Pegando os últimos 3 elementos
sub_tupla = tupla[-3:]
print(sub_tupla)  # Vai imprimir (4, 5, 6)
```

**Explicação**: O **fatiamento** (`tupla[1:4]`) permite que você extraia uma parte da tupla, da posição 1 até a 3 (a última posição não é incluída). O fatiamento pode ser usado com índices positivos e negativos para extrair dados de qualquer parte da tupla.

---

### 5. **Tupla com desempacotamento**

**Desempacotamento** de tuplas significa pegar os valores da tupla e armazená-los em variáveis individuais.

```python
pessoa = ("Maria", 30, "Engenheira")

# Desempacotando os valores da tupla
nome, idade, profissao = pessoa

print(f"Nome: {nome}, Idade: {idade}, Profissão: {profissao}")
# Vai imprimir "Nome: Maria, Idade: 30, Profissão: Engenheira"
```

**Explicação**: O desempacotamento permite que você **extraia os elementos** de uma tupla e os atribua diretamente a variáveis. Isso é muito útil quando você tem uma tupla com múltiplos valores e quer usá-los separadamente.

---

### **Resumo**

* **Tuplas** são sequências de dados **ordenados** e **imutáveis**.
* Elas são criadas com parênteses `()`.
* Você pode armazenar diferentes tipos de dados em uma tupla, como números, strings e até listas.
* **Tuplas** são úteis quando você **não quer que os dados sejam alterados** após serem criados.
* Operações como **acesso por índice**, **fatiamento** e **desempacotamento** são comuns com tuplas.

Tuplas são bastante usadas em Python, especialmente quando você quer armazenar dados que **não devem ser modificados** ao longo do tempo.

### Exemplo Prático: **Cadastro de Pessoa em uma Tupla**

Neste exemplo, vamos criar um programa onde o usuário insere seu **nome**, **idade** e **profissão**. Esses dados serão armazenados em uma **tupla** e, depois, serão exibidos de forma organizada.

```python
# Solicitando os dados ao usuário
nome = input("Digite seu nome: ")
idade = int(input("Digite sua idade: "))
profissao = input("Digite sua profissão: ")

# Criando uma tupla com os dados inseridos
pessoa = (nome, idade, profissao)

# Exibindo a tupla completa
print("\nDados cadastrados:")
print(f"Tupla de dados: {pessoa}")

# Desempacotando os dados da tupla
nome_tupla, idade_tupla, profissao_tupla = pessoa

# Exibindo os dados de forma legível
print(f"\nNome: {nome_tupla}")
print(f"Idade: {idade_tupla} anos")
print(f"Profissão: {profissao_tupla}")
```

### **Passo a Passo do Código:**

1. **Entrada de dados**: O programa solicita ao usuário que insira seu **nome**, **idade** e **profissão**.
2. **Criação da tupla**: Depois que o usuário digita as informações, essas são armazenadas em uma **tupla** chamada `pessoa`.
3. **Exibição da tupla**: O programa exibe a tupla inteira com todos os dados inseridos.
4. **Desempacotamento**: Em seguida, o código usa o **desempacotamento de tupla** para separar os dados em variáveis individuais: `nome_tupla`, `idade_tupla` e `profissao_tupla`.
5. **Exibição organizada**: Por fim, os dados são exibidos de forma legível, em formato de texto, usando as variáveis que foram extraídas da tupla.

### **Exemplo de Execução:**

**Entrada:**

```
Digite seu nome: João
Digite sua idade: 30
Digite sua profissão: Engenheiro
```

**Saída:**

```
Dados cadastrados:
Tupla de dados: ('João', 30, 'Engenheiro')

Nome: João
Idade: 30 anos
Profissão: Engenheiro
```

### **Explicação**:

* **Tupla**: A tupla `pessoa` contém os três dados inseridos pelo usuário: `("João", 30, "Engenheiro")`. A tupla é imutável, ou seja, não podemos alterar os dados dela diretamente, mas podemos usá-la para armazenar e manipular informações de forma organizada.
* **Desempacotamento**: O código mostra como separar os valores da tupla em variáveis individuais para facilitar o uso e exibição desses dados.

Embora não possamos **alterar** os elementos de uma tupla depois de criada, podemos **criar uma nova tupla** com dados atualizados, se necessário, ou até mesmo **transformar uma lista** em uma tupla, caso precisemos modificar os dados.


