### O que são **Conjuntos (Sets)**? 🧩

Em Python, um **conjunto (set)** é uma coleção de **elementos únicos** e **não ordenados**. Ou seja, um conjunto não permite **duplicatas** e não garante uma ordem específica dos elementos.

### Características dos **Conjuntos**:

* **Elementos únicos**: Um conjunto não permite elementos repetidos. Se você tentar adicionar um item que já existe no conjunto, ele será **ignorando**.
* **Desordenado**: O Python não garante a ordem dos elementos. Ou seja, quando você imprime um conjunto, a ordem pode ser diferente da ordem em que os elementos foram adicionados.
* **Mutáveis**: Você pode **adicionar** ou **remover** elementos de um conjunto.

### Como criar um **Conjunto**?

Em Python, os conjuntos são criados usando **chaves** `{}` ou a função `set()`.

```python
conjunto = {1, 2, 3, 4, 5}  # Criando um conjunto com números
```

Ou, você pode criar um conjunto vazio usando `set()`:

```python
conjunto_vazio = set()  # Conjunto vazio
```

---

### 1. **Exemplo Básico: Criando um conjunto**

Vamos começar com a criação de um conjunto e a verificação de seus elementos.

```python
conjunto = {1, 2, 3, 4, 5}

# Exibindo o conjunto
print(conjunto)  # Vai imprimir {1, 2, 3, 4, 5}
```

**Explicação**: O conjunto `conjunto` contém os elementos `1`, `2`, `3`, `4` e `5`. A ordem dos elementos não é garantida, então, se você imprimir o conjunto novamente, a ordem dos elementos pode mudar.

---

### 2. **Exemplo com eliminação de duplicatas**

Como um conjunto **não permite duplicatas**, ele vai automaticamente remover elementos repetidos quando você tentar adicioná-los.

```python
conjunto = {1, 2, 3, 3, 4, 5, 5}

# Exibindo o conjunto
print(conjunto)  # Vai imprimir {1, 2, 3, 4, 5}, duplicatas foram removidas
```

**Explicação**: Ao criar o conjunto com elementos repetidos (`3` e `5`), o Python automaticamente remove os duplicados, resultando em `{1, 2, 3, 4, 5}`.

---

### 3. **Exemplo com adição de elementos**

Você pode **adicionar** novos elementos a um conjunto utilizando o método `.add()`.

```python
conjunto = {1, 2, 3, 4}

# Adicionando um novo elemento
conjunto.add(5)

# Exibindo o conjunto após adicionar o novo elemento
print(conjunto)  # Vai imprimir {1, 2, 3, 4, 5}
```

**Explicação**: O método `.add()` é usado para adicionar um único elemento ao conjunto. Se você tentar adicionar um valor que já existe, ele será ignorado (sem duplicatas).

---

### 4. **Exemplo com remoção de elementos**

Você pode **remover** elementos de um conjunto usando o método `.remove()` ou `.discard()`.

* **`.remove()`**: Remove o elemento especificado, mas **gera um erro** se o elemento não existir.
* **`.discard()`**: Remove o elemento especificado, mas **não gera erro** se o elemento não existir.

```python
conjunto = {1, 2, 3, 4, 5}

# Removendo o número 3
conjunto.remove(3)

# Exibindo o conjunto após remoção
print(conjunto)  # Vai imprimir {1, 2, 4, 5}

# Tentando remover um número que não existe
conjunto.remove(6)  # Isso geraria um erro, porque 6 não está no conjunto
```

**Explicação**: O método `.remove()` remove o item especificado. Se o item não existir, ele gera um erro. Caso você queira evitar isso, use `.discard()`.

---

### 5. **Exemplo com operações entre conjuntos**

Os conjuntos permitem realizar **operações matemáticas**, como **união**, **interseção**, **diferença** e **diferença simétrica**.

#### **União** (`|` ou `.union()`): Combina os elementos de dois conjuntos.

```python
conjunto1 = {1, 2, 3}
conjunto2 = {3, 4, 5}

uniao = conjunto1 | conjunto2  # Usando o operador de união
print(uniao)  # Vai imprimir {1, 2, 3, 4, 5}
```

#### **Interseção** (`&` ou `.intersection()`): Retorna os elementos que estão em ambos os conjuntos.

```python
interseccao = conjunto1 & conjunto2  # Usando o operador de interseção
print(interseccao)  # Vai imprimir {3}
```

#### **Diferença** (`-` ou `.difference()`): Retorna os elementos que estão no primeiro conjunto, mas não no segundo.

```python
diferenca = conjunto1 - conjunto2  # Usando o operador de diferença
print(diferenca)  # Vai imprimir {1, 2}
```

#### **Diferença Simétrica** (`^` ou `.symmetric_difference()`): Retorna os elementos que estão em **apenas um** dos conjuntos (sem repetições).

```python
diferenca_simetrica = conjunto1 ^ conjunto2  # Usando o operador de diferença simétrica
print(diferenca_simetrica)  # Vai imprimir {1, 2, 4, 5}
```

**Explicação**: Esses operadores e métodos permitem **comparar conjuntos** e obter resultados baseados na combinação ou diferença de seus elementos. As operações são bastante úteis quando você trabalha com conjuntos de dados e precisa realizar **análises comparativas**.

---

### **Resumo**

* **Conjunto (Set)**: Uma coleção de elementos **únicos** e **não ordenados**.
* **Mutável**: Você pode **adicionar**, **remover** e **modificar** elementos.
* **Elementos Únicos**: Não permite **duplicatas**.
* **Operações**: Você pode fazer operações como **união**, **interseção**, **diferença** e **diferença simétrica** entre conjuntos.

---

### **Exemplo Completo com Conjuntos**

```python
# Criando dois conjuntos
conjunto1 = {1, 2, 3, 4}
conjunto2 = {3, 4, 5, 6}

# Adicionando elementos
conjunto1.add(7)

# Removendo elementos
conjunto2.remove(6)

# Exibindo o resultado das operações
print("União:", conjunto1 | conjunto2)  # União
print("Interseção:", conjunto1 & conjunto2)  # Interseção
print("Diferença:", conjunto1 - conjunto2)  # Diferença
print("Diferença Simétrica:", conjunto1 ^ conjunto2)  # Diferença simétrica
```

**Resultado Esperado**:

```
União: {1, 2, 3, 4, 5, 7}
Interseção: {3, 4}
Diferença: {1, 2}
Diferença Simétrica: {1, 2, 5, 7}
```
