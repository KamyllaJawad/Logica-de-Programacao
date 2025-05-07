### O que são **estruturas de dados**? 🗂️

**Estruturas de dados** são formas de **organizar e armazenar dados** em um computador de maneira eficiente. A maneira como você organiza os dados influencia como você pode acessá-los, modificá-los e manipulá-los.

Em outras palavras, uma **estrutura de dados** define a maneira como os dados são **organizados**, **armazenados** e **manipulados** no programa, permitindo que você execute operações como inserção, busca, atualização e exclusão de maneira mais eficiente.

### Por que são importantes? 🔑

Uma boa escolha de estrutura de dados pode **melhorar a performance** do seu programa, tornando as operações de busca, inserção e exclusão mais rápidas. Por exemplo, uma lista pode ser eficiente para acessar dados em sequência, mas se você precisar buscar elementos frequentemente, uma **pilha** ou **fila** pode ser mais adequada dependendo do caso.

### Tipos de Estruturas de Dados

Existem várias **estruturas de dados**. Vou explicar as mais comuns:

---

### 1. **Listas (List)** 📃

* **O que é?** Uma lista é uma **sequência ordenada** de elementos, que podem ser de qualquer tipo (números, strings, objetos, etc.).
* **Como funciona?** Em Python, as listas são representadas com colchetes `[]`.

**Exemplo:**

```python
frutas = ["maçã", "banana", "laranja"]
```

* Você pode **acessar**, **modificar**, **adicionar** ou **remover** elementos de uma lista.

**Operações comuns:**

```python
# Acessar o primeiro elemento
print(frutas[0])  # Vai imprimir "maçã"

# Adicionar um item
frutas.append("uva")

# Remover um item
frutas.remove("banana")
```

* **Vantagens:** Simples e muito usadas, fáceis de entender e trabalhar.
* **Desvantagens:** O desempenho para operações de **busca** pode ser lento, especialmente com listas grandes.

---

### 2. **Tuplas (Tuple)** 🧩

* **O que é?** Uma tupla é **semelhante a uma lista**, mas a principal diferença é que uma **tupla é imutável**. Ou seja, depois de criada, não podemos **alterar** seus elementos.
* **Como funciona?** As tuplas são representadas com parênteses `()`.

**Exemplo:**

```python
cores = ("vermelho", "azul", "verde")
```

* **Vantagens:** Como são imutáveis, tuplas podem ser mais eficientes em termos de memória.
* **Desvantagens:** Você não pode modificar os dados depois de criar a tupla.

**Operações comuns:**

```python
# Acessar o primeiro item
print(cores[0])  # Vai imprimir "vermelho"
```

---

### 3. **Dicionários (Dictionary)** 🔑

* **O que é?** Um **dicionário** é uma coleção de **pares chave-valor**. Ou seja, ele armazena os dados associados a uma chave, e você pode acessar o valor associado a essa chave.
* **Como funciona?** Os dicionários são representados com chaves `{}`.

**Exemplo:**

```python
aluno = {"nome": "João", "idade": 18, "curso": "Python"}
```

* **Vantagens:** Muito eficientes para **busca** de dados com base em uma chave.
* **Desvantagens:** Não mantêm a ordem dos elementos (em versões mais antigas do Python, mas a partir da versão 3.7, eles são **ordenados**).

**Operações comuns:**

```python
# Acessar um valor pela chave
print(aluno["nome"])  # Vai imprimir "João"

# Adicionar um novo par chave-valor
aluno["nota"] = 9

# Remover um item
del aluno["idade"]
```

---

### 4. **Conjuntos (Set)** 🧩

* **O que é?** Um **conjunto** é uma coleção de elementos **únicos**. Ou seja, não pode haver elementos repetidos.
* **Como funciona?** Os conjuntos são representados com chaves `{}`, assim como os dicionários, mas **não têm chave-valor**.

**Exemplo:**

```python
numeros = {1, 2, 3, 4, 5}
```

* **Vantagens:** Muito eficientes para operações de **verificação de pertencimento** (verificar se um item está presente).
* **Desvantagens:** Não permitem elementos duplicados e não mantêm a ordem dos elementos.

**Operações comuns:**

```python
# Verificar se um item existe no conjunto
print(3 in numeros)  # Vai imprimir True

# Adicionar um novo item
numeros.add(6)

# Remover um item
numeros.remove(4)
```

---

### 5. **Pilhas (Stack)** 📦

* **O que é?** Uma pilha é uma estrutura de dados que segue o princípio **LIFO** (Last In, First Out), ou seja, o último item a ser inserido é o primeiro a ser retirado.
* **Como funciona?** Você pode adicionar itens no topo da pilha e remover apenas o item do topo.

**Exemplo:**

```python
pilha = []
pilha.append(1)  # Empilha 1
pilha.append(2)  # Empilha 2
pilha.pop()      # Desempilha (remove o 2)
```

* **Vantagens:** Útil para situações em que você precisa de um comportamento de **último a entrar, primeiro a sair**.
* **Desvantagens:** Não é eficiente se você precisar acessar ou remover elementos no meio da pilha.

---

### 6. **Filas (Queue)** ⏳

* **O que é?** Uma fila segue o princípio **FIFO** (First In, First Out), ou seja, o primeiro item a ser inserido será o primeiro a ser retirado.
* **Como funciona?** Você pode adicionar itens ao final da fila e remover itens do início.

**Exemplo:**

```python
fila = []
fila.append("A")  # Enfileira "A"
fila.append("B")  # Enfileira "B"
fila.pop(0)        # Desenfileira "A"
```

* **Vantagens:** Útil quando você quer **processar itens na ordem em que foram recebidos**.
* **Desvantagens:** Não é eficiente se você precisar acessar itens no meio da fila.

---

### 7. **Árvores (Tree)** 🌳

* **O que é?** Uma **árvore** é uma estrutura hierárquica onde cada elemento é chamado de **nó**. O nó superior é chamado de **raiz**, e cada nó pode ter **filhos** (nós conectados a ele).
* **Como funciona?** Árvores são úteis para representar hierarquias, como estrutura de pastas em um computador ou relações familiares.

**Exemplo:**

```python
class Node:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

root = Node(10)  # Raiz da árvore
root.left = Node(5)  # Filho à esquerda
root.right = Node(15)  # Filho à direita
```

* **Vantagens:** Útil para armazenar dados hierárquicos e fazer buscas rápidas.
* **Desvantagens:** Mais complexa de implementar e manipular.

---

### Conclusão

As **estruturas de dados** são fundamentais para qualquer programador, pois permitem organizar e manipular dados de maneira eficiente. O tipo de estrutura que você usa depende do problema que está tentando resolver e das operações que precisa realizar frequentemente.

Aqui está um resumo das **estruturas de dados** que vimos:

* **Listas (List):** Sequência ordenada de elementos.
* **Tuplas (Tuple):** Sequência ordenada e imutável de elementos.
* **Dicionários (Dictionary):** Coleção de pares chave-valor.
* **Conjuntos (Set):** Coleção de elementos únicos.
* **Pilhas (Stack):** Estrutura LIFO (último a entrar, primeiro a sair).
* **Filas (Queue):** Estrutura FIFO (primeiro a entrar, primeiro a sair).
* **Árvores (Tree):** Estrutura hierárquica de nós.

Cada uma tem suas **vantagens** e **desvantagens**, e você deve escolher a estrutura certa dependendo do que precisa fazer no seu programa.


