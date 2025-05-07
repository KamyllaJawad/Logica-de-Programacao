### O que são **Árvores**? 🌳

Uma **árvore** é uma estrutura de dados hierárquica composta por **nós** (também chamados de **nós de árvore**). Cada nó pode ter **filhos** e pode ser **conectado** a outros nós.

#### Componentes de uma árvore:

* **Raiz** (Root): O nó principal ou inicial da árvore, que não tem nenhum nó pai.
* **Nó** (Node): Cada item ou estrutura dentro da árvore. Pode ser um valor qualquer.
* **Filho** (Child): Um nó que está abaixo de outro nó na árvore.
* **Pai** (Parent): Um nó que está acima de outro nó.
* **Folha** (Leaf): Um nó que não tem filhos.
* **Profundidade** (Depth): A distância entre a raiz e o nó.
* **Altura** (Height): A distância entre um nó e a folha mais distante.

### Como funcionam as **Árvores**?

As árvores são representadas de forma hierárquica, com a **raiz** no topo e os nós se ramificando para formar uma estrutura em árvore. Uma árvore pode ter vários filhos e filhas, formando **subárvores**.

### Tipos de Árvores:

1. **Árvore Binária**: Cada nó tem no máximo dois filhos, chamados de **filho esquerdo** e **filho direito**.
2. **Árvore N-ária**: Cada nó pode ter N filhos, podendo ser mais de dois.
3. **Árvore de Pesquisa Binária**: Árvores binárias com uma propriedade onde a chave do filho esquerdo é menor que a chave do pai, e a chave do filho direito é maior que a chave do pai.

Vamos começar com uma explicação prática de **Árvore Binária**.

---

### **Exemplo Básico de Árvore Binária**

Em uma **árvore binária**, cada nó tem **até dois filhos** (um à esquerda e um à direita). Aqui está um exemplo de como representar uma árvore binária simples:

```python
class Node:
    def __init__(self, value):
        self.value = value  # O valor do nó
        self.left = None    # Filho esquerdo
        self.right = None   # Filho direito

# Criando a árvore
root = Node(10)  # Raiz da árvore com o valor 10
root.left = Node(5)  # Filho esquerdo da raiz com o valor 5
root.right = Node(15)  # Filho direito da raiz com o valor 15
root.left.left = Node(3)  # Filho esquerdo do nó 5 com o valor 3
root.left.right = Node(7)  # Filho direito do nó 5 com o valor 7
```

**Explicação**:

* O nó **raiz** tem o valor 10.
* O nó **esquerdo** da raiz tem o valor 5.
* O nó **direito** da raiz tem o valor 15.
* O nó **esquerdo** de 5 tem o valor 3 e o nó **direito** de 5 tem o valor 7.

Aqui temos uma árvore binária simples, que se parece com isso:

```
       10
      /  \
     5    15
    / \
   3   7
```

---

### **Exemplo de Traversal (Percurso da Árvore)**

Existem **vários tipos de percursos** (traversals) em uma árvore. Vamos ver os mais comuns: **pré-ordem**, **in-ordem** e **pós-ordem**.

* **Pré-ordem**: Visita o nó **antes** de seus filhos.
* **In-ordem**: Visita o nó **entre** os filhos esquerdo e direito.
* **Pós-ordem**: Visita o nó **após** seus filhos.

#### Exemplo de **Percurso em Pré-Ordem**:

```python
def pre_order(node):
    if node:
        print(node.value, end=" ")  # Primeiro visita o nó
        pre_order(node.left)  # Depois visita o filho esquerdo
        pre_order(node.right)  # Depois visita o filho direito

pre_order(root)  # Vai imprimir: 10 5 3 7 15
```

**Explicação**: O **pré-ordem** visita o nó antes de visitar seus filhos, começando pela raiz e indo para os filhos da esquerda, e depois os filhos da direita.

#### Exemplo de **Percurso em In-Ordem**:

```python
def in_order(node):
    if node:
        in_order(node.left)  # Visita o filho esquerdo
        print(node.value, end=" ")  # Visita o nó
        in_order(node.right)  # Visita o filho direito

in_order(root)  # Vai imprimir: 3 5 7 10 15
```

**Explicação**: O **in-ordem** visita os nós da árvore em ordem crescente (para árvores binárias de pesquisa). Primeiro, visita todos os filhos esquerdos, depois o nó, e depois os filhos direitos.

#### Exemplo de **Percurso em Pós-Ordem**:

```python
def post_order(node):
    if node:
        post_order(node.left)  # Visita o filho esquerdo
        post_order(node.right)  # Visita o filho direito
        print(node.value, end=" ")  # Visita o nó

post_order(root)  # Vai imprimir: 3 7 5 15 10
```

**Explicação**: O **pós-ordem** visita os filhos antes de visitar o nó. Primeiro visita todos os filhos esquerdo e direito, e só depois visita o nó em si.

---

### **Exemplo Completo: Árvore Binária de Pesquisa (BST)**

Em uma **Árvore Binária de Pesquisa (BST)**, para cada nó:

* O valor do **filho esquerdo** é **menor** que o valor do nó.
* O valor do **filho direito** é **maior** que o valor do nó.

Vamos criar uma árvore binária de pesquisa simples:

```python
class BSTNode:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

# Inserção na árvore binária de pesquisa
def insert(root, value):
    if root is None:
        return BSTNode(value)
    else:
        if value < root.value:
            root.left = insert(root.left, value)
        else:
            root.right = insert(root.right, value)
    return root

# Criando a árvore
root = BSTNode(10)
root = insert(root, 5)
root = insert(root, 15)
root = insert(root, 3)
root = insert(root, 7)
root = insert(root, 12)
root = insert(root, 18)

# Exibindo a árvore em in-ordem
in_order(root)  # Vai imprimir: 3 5 7 10 12 15 18
```

**Explicação**:

* Começamos com a raiz `10`.
* Inserimos `5`, `15`, `3`, `7`, `12`, e `18` de acordo com as regras de uma árvore binária de pesquisa.
* A função **`insert`** insere o valor na posição correta, comparando com o valor do nó atual, e recursivamente vai para a esquerda ou direita.

---

### **Conclusão e Resumo**

* **Árvore Binária**: Cada nó tem **até dois filhos**, um à esquerda e outro à direita. A **ordem de visitação** pode ser feita de diferentes maneiras: **pré-ordem**, **in-ordem** e **pós-ordem**.
* **Árvore Binária de Pesquisa (BST)**: Uma árvore onde, para cada nó, o **valor à esquerda é menor** e o **valor à direita é maior**.
* **Percursos (Traversals)**: O percurso em **pré-ordem**, **in-ordem** e **pós-ordem** permite visitar os nós de diferentes maneiras.
* **Operações**: As árvores são usadas para **buscas eficientes**, **inserções** e **remoções** em várias aplicações.

---

### **Exemplo Completo com Árvore Binária de Pesquisa**

Aqui está um código completo que cria uma **Árvore Binária de Pesquisa (BST)**, insere alguns valores e faz o percurso **in-ordem**:

```python
class BSTNode:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

# Função de inserção na árvore binária de pesquisa
def insert(root, value):
    if root is None:
        return BSTNode(value)
    if value < root.value:
        root.left = insert(root.left, value)
    else:
        root.right = insert(root.right, value)
    return root

# Função de percurso em in-ordem
def in_order(node):
    if node:
        in_order(node.left)
        print(node.value, end=" ")
        in_order(node.right)

# Criando a árvore e inserindo valores
root = BSTNode(10)
root = insert(root, 5)
root = insert(root, 15)
root = insert(root, 3)
root = insert(root, 7)
root = insert(root, 12)
root = insert(root, 18)

# Exibindo os valores da árvore em in-ordem
print("Árvore em in-ordem:")
in_order(root)  # Vai imprimir: 3 5 7 10 12 15 18
```

Esse código cria uma árvore binária de pesquisa, insere os valores em ordem e exibe o resultado em ordem crescente.

